document.getElementById('searchInput').addEventListener('input', function () {
    const query = this.value.toLowerCase();
    const posts = document.querySelectorAll('.post');
    posts.forEach(post => {
        const text = post.innerText.toLowerCase();
        post.style.display = text.includes(query) ? 'block' : 'none';
    });
});
