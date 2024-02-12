// Example JavaScript functions for posting and searching

// Simulated user data and posts
const currentUser = { username: "exampleUser" };
const posts = [];

function postContent() {
    const postContent = document.getElementById("postContent").value;
    if (postContent.trim() !== "") {
        const post = {
            user: currentUser.username,
            content: postContent,
            likes: 0,
        };
        posts.push(post);
        displayPosts();
        document.getElementById("postContent").value = "";
    }
}

function likePost(index) {
    posts[index].likes++;
    displayPosts();
}

function displayPosts() {
    const userPostsContainer = document.getElementById("userPosts");
    userPostsContainer.innerHTML = "";
    posts.forEach((post, index) => {
        const postElement = document.createElement("div");
        postElement.innerHTML = `<p class="post"><strong>${post.user}</strong>: ${post.content}</p>
                                  <button class="like-button" onclick="likePost(${index})">Like (${post.likes})</button>`;
        userPostsContainer.appendChild(postElement);
    });
}

function searchUser() {
    const searchTerm = document.getElementById("searchUser").value.toLowerCase();
    const searchResultsContainer = document.getElementById("searchResults");
    const results = posts.filter(post => post.user.toLowerCase().includes(searchTerm));
    searchResultsContainer.innerHTML = "";
    results.forEach(result => {
        const resultElement = document.createElement("div");
        resultElement.innerHTML = `<p class="search-result"><strong>${result.user}</strong></p>`;
        searchResultsContainer.appendChild(resultElement);
    });
}
