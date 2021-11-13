# Budget-Tracker

## Deployed Link
https://budget-tracker-mehdi.herokuapp.com/

## Summary
This is a budget tracking app, you can add money, or substract money from your virtual account, and track the data in your dashboard.

## Link To Deployed App
https://polar-badlands-25931.herokuapp.com/#

## Screenshot Of Main Screen
<img width="1127" alt="Screenshot 2021-11-12 at 16 41 22" src="https://user-images.githubusercontent.com/75599021/141598970-7f922775-7b99-4f83-8390-e1e9dcf59d88.png">

## Built With
* [Javascript](https://developer.mozilla.org/en-US/docs/Web/JavaScript)
* [Node.js](https://nodejs.org/en/docs/)
* [NPM-Library](https://docs.npmjs.com/)
* [Expres.js](https://expressjs.com/)
* [Sequelize](https://sequelize.org/master/index.html)
* [mongodb](https://www.mongodb.com/)

## Installation Steps For Local Running
1. Clone project.
2. Open terminal and run these commands in order
    - npm install
    - npm run seed
    - npm start

## Code Snippet Adding Transaction
```javascript
router.post("/api/transaction", ({ body }, res) => {
  Transaction.create(body)
    .then(dbTransaction => {
      res.json(dbTransaction);
    })
    .catch(err => {
      res.status(400).json(err);
    });
});

```

## Author

* **Mehdi Safari**

- [Link to Portfolio Site](https://mehdisafari77.github.io/Basic-Bio/)
- [Link to Github](https://github.com/mehdisafari77)
- [Link to LinkedIn](https://www.linkedin.com/in/mehdi-safari-992799142/)
