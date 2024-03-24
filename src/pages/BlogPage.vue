<template>
  <Div class="title1">
    <h3>-Bolg posts-</h3>
  </Div>
  <!-- Blog Post Cards -->
  <div class="blog-post-cards">
    <div class="row justify-center">
      <div v-for="(post, index) in blogPosts" :key="index" class="col-md-5">
        <div class="blog-post-card">
          <img :src="post.imageSrc" alt="Post Image" class="post-image" />
          <div class="post-content">
            <h2 class="post-title">{{ post.title }}</h2>
            <p class="post-description">{{ post.description }}</p>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  data() {
    return {
      blogPosts: [
        {
          imageSrc:
            "https://cdn.pixabay.com/photo/2015/04/23/22/00/tree-736885_1280.jpg",
          title: "Post 1",
          description: "Description for Post 1",
        },
        {
          imageSrc:
            "https://img.lovepik.com/background/20211022/large/lovepik-sky-clouds-background-image_401746897.jpg",
          title: "Post 2",
          description: "Description for Post 2",
        },
        {
          imageSrc:
            "https://img.lovepik.com/background/20211022/large/lovepik-sky-clouds-background-image_401746897.jpg",
          title: "Post 3",
          description: "Description for Post 2",
        },
        {
          imageSrc:
            "https://img.lovepik.com/background/20211022/large/lovepik-sky-clouds-background-image_401746897.jpg",
          title: "Post 4",
          description: "Description for Post 2",
        },
        // Add more blog posts as needed to fill the 10 cards
      ],
    };
  },
};
</script>
<style scoped>
* {
  margin: 0;
  padding: 0;
}
body {
  background-color: #b71818 !important;
}

.blog-post-cards {
  /* Add styles for the blog post cards container here */
  margin-top: 20px;
}

/* Style for each individual blog post card */
.blog-post-card {
  width: 600px; /* Set a fixed width for the card */
  height: 400px; /* Set a fixed height for the card */
  padding: 10px;
  border: 1px solid #ccc;
  border-radius: 5px;
  box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
  margin-bottom: 20px;
  overflow: hidden; /* Hide overflow content */
  transition: transform 0.3s ease; /* Add transition for smooth effect */
}

.blog-post-card:hover {
  transform: scale(1.1); /* Scale the card on hover */
  background-color: rgb(213, 208, 208);
}

/* Style for post image */
.post-image {
  width: 100%;
  height: 250px; /* Set a fixed height for the image */
  object-fit: cover; /* Ensure the image covers the container */
}

/* Style for post content */
.post-content {
  padding: 10px;
}

/* Style for post title */
.post-title {
  margin-top: 5px;
  font-size: 16px;
  font-weight: bold;
}

/* Style for post description */
.post-description {
  margin-top: 5px;
  font-size: 14px;
}
.title1 {
  text-align: center;
  margin-top: 20px;
}
</style>
