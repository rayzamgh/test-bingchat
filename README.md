# test-bingchat
free test API for bingchat

# Run this every so often:
```
const cookie = document.cookie;
const serverUrl = "https://bingchat-api-zmtik7wuba-et.a.run.app";

fetch(`${serverUrl}/set-cookie`, {
  method: "POST",
  headers: {
    "Content-Type": "application/json",
  },
  body: JSON.stringify({ cookie }),
})
  .then((res) => res.json())
  .then((res) => console.log(res))
  .catch((err) => console.log(err));
```
