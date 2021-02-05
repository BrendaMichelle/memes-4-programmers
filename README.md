# Meme App

## Set up

- Fork and clone this repository.
- Install JSON Server if you haven't already by running `npm install -g json-server` in your terminal
- Start the JSON Server by running `json-server --watch db.json` in your terminal
- If you go to ` http://localhost:3000/posts`, you'll see all the posts. This is the URL, you'll want to make a `get` request to in order to get all the meme posts, for example. The available routes include:

        - POST /posts
        - DELETE /posts/:id
        - PATCH /posts/:id
        - GET /posts

## Deliverables:

- User should see all memes rendered in the `div#listings` when the page loads. Each meme post should look like this:
```HTML
<div class="post">
    <div class="image">
        <img src="{meme url}">
        <button class="delete-button">X</button>
    </div>
    <h4 class="description">{meme description}!</h4>
    <p class="likes-count">{meme likes}</p>
    <button class="likes-button" data-button-type="upvote">👍</button>
<div>
```

- User should be able to create a new meme. The new meme should display on the page without a page reload, but should still persist if the page reloads.

- User should be able to upvote a meme when they click on the `👍` button. The likes should persist.

- User should be able to delete a meme when they click on the `X` button. The deleted meme should not re-appear on the webpage when the page reloads.
