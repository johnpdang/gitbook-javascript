# API

|                                                                                                                                                                                                                                              |         |
| -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------- |
| [What is API & REST API ?](https://dev.to/parmita17/what-is-api-rest-api--3noe)                                                                                                                                                              | 9/10/23 |
| [10 Web APIs Every Senior Web Engineer Should Master!](https://javascript.plainenglish.io/10-web-apis-every-senior-web-engineer-should-master-8ef3198368c2)                                                                                  | 7/9/23  |
| [7 More JavaScript Web APIs to Build Futuristic Websites you didn't Know 🤯](https://dev.to/ruppysuppy/7-more-javascript-web-apis-to-build-futuristic-websites-you-didnt-know-50bg)                                                          | 6/28/23 |
| [Watching for changes to a user's location](https://gomakethings.com/watching-for-changes-to-a-users-location/)                                                                                                                              | 6/27    |
| [How to setup a middleman API with vanilla JS](https://gomakethings.com/how-to-setup-a-middleman-api-with-vanilla-js/)                                                                                                                       | 5/1     |
| [API credentials and security with vanilla JS](https://gomakethings.com/api-credentials-and-security-with-vanilla-js/)                                                                                                                       | 4/29    |
| [API authentication with vanilla JS](https://gomakethings.com/api-authentication-with-vanilla-js/)                                                                                                                                           | 4/28    |
| [How to Use the Web Storage API](https://blog.bitsrc.io/localstorage-sessionstorage-the-web-storage-of-the-web-6b7ca51c8b2a)                                                                                                                 | 2/21    |
| [How to Detect When a Sticky Element Gets Pinned](https://davidwalsh.name/detect-sticky?utm\_source=Responsive+Design+Weekly\&utm\_campaign=f46addca91-RWD\_Newsletter\_435\&utm\_medium=email\&utm\_term=0\_df65b6d7c8-f46addca91-59185629) | 11/13   |

### [API](https://developer.mozilla.org/en-US/docs/Web/API)

|                                                                                      |                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        |
| ------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| [localStorage](https://developer.mozilla.org/en-US/docs/Web/API/Window/localStorage) | The read-only **`localStorage`** property allows you to access a [`Storage`](https://developer.mozilla.org/en-US/docs/Web/API/Storage) object for the [`Document`](https://developer.mozilla.org/en-US/docs/Web/API/Document)'s origin; the stored data is saved across browser sessions. `localStorage` is similar to [`sessionStorage`](https://developer.mozilla.org/en-US/docs/Web/API/Window/sessionStorage), except that while data stored in `localStorage` has no expiration time, data stored in `sessionStorage` gets cleared when the page session ends — that is, when the page is closed. |
| [fetch](https://developer.mozilla.org/en-US/docs/Web/API/Fetch\_API)                 | The Fetch API provides an interface for fetching resources (including across the network). It will seem familiar to anyone who has used [`XMLHttpRequest`](https://developer.mozilla.org/en-US/docs/Web/API/XMLHttpRequest), but the new API provides a more powerful and flexible feature set.                                                                                                                                                                                                                                                                                                        |

```javascript
    const baseEndpoint = 'https://api.github.com';
    const usersEndpoint = `${baseEndpoint}/users`;
    const userEl = document.querySelector('.user');

    async function displayUser(username) {
      userEl.textContent = 'loading...';
      const response = await fetch(`${usersEndpoint}/${username}`);
      const data = await response.json();
      console.log(data);
      console.log(data.blog);
      console.log(data.name);
      console.log(data.location);
      userEl.textContent = `${data.name} - ${data.blog}`;
    }

    function handleError(err) {
      console.log('OH NO!');
      console.log(err);
      userEl.textContent = `Something went wrong: ${err}`
    }

    displayUser('stolinski').catch(handleError);
```

|                                                                                          |   |
| ---------------------------------------------------------------------------------------- | - |
| [http://api.github.com/users/johnpdang](http://api.github.com/users/johnpdang)           |   |
| [https://exchangeratesapi.io/](https://exchangeratesapi.io/)                             |   |
| [https://github.com/public-apis/public-apis](https://github.com/public-apis/public-apis) |   |
| [https://icanhazdadjoke.com/api](https://icanhazdadjoke.com/api)                         |   |
| [http://recipepuppy.com/api](http://recipepuppy.com/api)                                 |   |

```javascript
http://recipepuppy.com/api/

//parameters
?
i=onions,garlic //ingredients
&
q=omelet //query
&
p=3 //pagination


```
