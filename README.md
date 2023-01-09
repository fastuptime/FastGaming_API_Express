# FastGaming_API_Express

## Usage/Examples

![image](https://user-images.githubusercontent.com/63351166/211326748-43b9471d-173f-4cd0-a6ae-be4238ad82a6.png)

```javascript
  var axios = require("axios");
  var qs = require("qs");
  var data = qs.stringify({
    type: "minecraft",
    host: "play.craftrise.com.tr",
  });
  var config = {
    method: "post",
    url: "http://localhost/api",
    headers: {
      Accept: "application/json",
      "Content-Type": "application/x-www-form-urlencoded",
    },
    data: data,
  };

  axios(config)
    .then(function (response) {
      console.log(JSON.stringify(response.data));
    })
    .catch(function (error) {
      console.log(error);
    });
```


## API Reference

```http
  POST /api
```

- Form Data

| Parameter | Type     | Description                       |
| :-------- | :------- | :-------------------------------- |
| `type`      | `string` | Server ID in game_list.txt |

| Parameter | Type     | Description                       |
| :-------- | :------- | :-------------------------------- |
| `host`      | `string`,| Server ip address |

## Tech Stack

**Server:** Node, Express, Gamedig

---
- ✨ [Destek İçin](https://fastuptime.com) <br>
- 💕 [Discord](https://fastuptime.com/discord)<br>
- 🎖️ [FasterHost Technology](https://fasterhost.tech/)<br>
- ✨ İletişim için [Tıkla!](mailto:fastuptime@gmail.com)<br>

# License
- Its protected by Creative Commons ([CC BY-NC-SA 4.0](https://creativecommons.org/licenses/by-nc-sa/4.0/))

<a href="https://creativecommons.org/licenses/by-nc-sa/4.0/" title="BYNCSA40"><img src="https://licensebuttons.net/l/by-nc-sa/4.0/88x31.png"></a>
