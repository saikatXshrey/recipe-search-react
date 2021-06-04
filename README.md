

Uploading Recipe Search - Google Chrome 2021-06-04 13-26-30.mp4…


# Food Search React

This app helps you find "food-items" based on the search keyword provided by you during search

And displays all the possible outcomes of "food-items" and displays it in an orderly manner in cards which contains (item name,item ingredients,item image & item calorie)

Makes more options avaliable to prepare dish you want



## Demo

Insert gif or link to demo

  
## Screenshots

![App Screenshot](https://via.placeholder.com/468x300?text=App+Screenshot+Here)

  
## API Reference

Api used is [Edamam](https://www.edamam.com/)

#### Get all items

```http
  GET /api/items

 `https://api.edamam.com/search?q=${search_keyword}&app_id=${YOUR_APP_ID}&app_key=${YOUR_APP_KEY}`
```

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `search_keyword` | `string` | **Required**. Consumer Search keyword |

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `api_id` | `string` | **Required**. Your API id |


| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `api_key` | `string` | **Required**. Your API key |


  
## Environment Variables

To run this project, you will need to add the following environment variables to your .env file or in a const variable

`YOUR_EDAMAM_API_ID`

`YOUR_EDAMAM_API_KEY`

  
## Deployment

To deploy this project run

```bash
  npm run deploy
```

  
## Lessons Learned

This project is made using functional component and Hooks is used heavily in this project.
Particularly useState and useEffect and fetch api(fetch from api) and also working with api becomes more handy by making this project

The main problems that i had to overcome is state magament and as Edamam only supports 10 requests per minute i had to ensure that the app does not fetch everytime there's an onChange.
And finally resfreshing the search state everytime the user clicks the "Search" button.

  
