# IIT-BHU-CyberSecWeb-FrontEnd-API

## Frontend API for IIT(BHU)CyberSecWebsite

### How to run in Development mode
1. create `.env` file with 2 variables `DB_USERNAME` and `DB_PASSWORD` and set them according to your MongoDB Atlas username and password
2. Update the `mongoString` in `index.js` according to your mongoString.
3. Run `npm i` in the root directory
4. Seed the Database
5. Run `npm run dev` to start the API on `http://localhost:5000`

### Production
1. Currently the API is hosted at https://api-iitbhucybersec-main.herokuapp.com/
2. Any pushes to the main branch of this repo will be reflected upon this URL
3. `.env` is configured to use the IIT(BHU)CyberSec account of MongoDB

### Seeding the Database
1. Create a cluster in mongoDB
2. Allow access from all IP's (or only your IP if you wish to)
3. Create a Database and updated your `mongoString` accordingly
4. Create a collection in the database called blogdb
5. add the following JSON data to that collection
```
[
  {
    "tags": ["react", "javascript"],
    "id": "Gk5IxHDUqZrY",
    "title": "How to Create a Website with Next.js & React",
    "urlTitle": "how-to-create-a-website-with-next-js-and-react",
    "dateTimestamp": 1583852400,
    "thumbnailImageUrl": "https://assets.coderrocketfuel.com/coding-blog-react-thumbnail.png",
    "markdownContent": "# Blog Post Content",
    "seoTitleTag": "How to Create a Website with Next.js & React | Coding Blog",
    "seoMetaDescription": "A complete guide on how to setup, configure, and build a website using the Next.js React framework."
  },
  {
    "tags": ["nodejs"],
    "id": "AdffVG6mcCAj",
    "title": "Create a REST API With NodeJS",
    "urlTitle": "create-a-rest-api-with-node-js",
    "dateTimestamp": 1584266400,
    "thumbnailImageUrl": "https://assets.coderrocketfuel.com/coding-blog-nodejs-thumbnail.png",
    "markdownContent": "# Blog Post Content",
    "seoTitleTag": "Create a REST API With NodeJS | Coding Blog",
    "seoMetaDescription": "A guide on how to build a REST API using Node.js and Express."
  },
  {
    "tags": ["css"],
    "id": "wGqjKfOR2Skm",
    "title": "How to Use the CSS calc() Function",
    "urlTitle": "how-to-use-the-css-calc-function",
    "dateTimestamp": 1583748000,
    "thumbnailImageUrl": "https://assets.coderrocketfuel.com/coding-blog-css-thumbnail.png",
    "markdownContent": "# Blog Post Content",
    "seoTitleTag": "How to Use the CSS calc() Function | Coding Blog",
    "seoMetaDescription": "Guide on how to use the CSS calc() function in CSS files."
  },
  {
    "tags": ["html"],
    "id": "AUaKWwFdNyPd",
    "title": "How to Put Spaces Between Text in HTML",
    "urlTitle": "how-to-put-spaces-between-text-in-html",
    "dateTimestamp": 1583406000,
    "thumbnailImageUrl": "https://assets.coderrocketfuel.com/coding-blog-html-thumbnail.png",
    "markdownContent": "# Blog Post Content",
    "seoTitleTag": "How to Put Spaces Between Text in HTML | Coding Blog",
    "seoMetaDescription": "Tutorial on adding spacing to HTML text with the <Pre> tag, HTML whitespace characters, and CSS empty span width and margin styling."
  },
  {
    "tags": ["git"],
    "id": "lFEB9v6kl75A",
    "title": "Introduction to Git - Background, Installation, and Usage",
    "urlTitle": "introduction-to-git-version-control-system",
    "dateTimestamp": 1584698400,
    "thumbnailImageUrl": "https://assets.coderrocketfuel.com/coding-blog-git-thumbnail.png",
    "markdownContent": "# Blog Post Content",
    "seoTitleTag": "Introduction to Git - Background, Installation, and Usage | Coding Blog",
    "seoMetaDescription": "Introduction to Git version control software. Learn about the background and get a guide on installing and using Git."
  }
]
```
