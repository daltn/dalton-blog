<template>
  <article class="container">
    <h1>art camp library</h1>
    <a
      href="https://artcamplibrary.com"
      target="_blank"
      rel="noopener noreferrer"
      >https://artcamplibrary.com</a
    >
    <p>
      Art Camp Library is a randomized art generator built in collaboration w/
      the design studio
      <a
        href="https://www.madeatartcamp.com/"
        rel="noopener noreferrer"
        target="_blank"
        >Art Camp</a
      >. It is an express app running on an AWS EC2 instance behind an NGINX
      reverse proxy. The images are all scans from the studio's book collection
      and the images are updated through an admin panel where they are uploaded
      to AWS S3 and the art piece's data flows to a SQLite db. I had a blast
      making this and return to it all the time to get visual inspiration.
    </p>
    <p>
      <a
        href="https://github.com/daltn/art-camp-lib"
        rel="noopener noreferrer"
        target="_blank"
        >source code</a
      >
    </p>
    <img src="~/assets/art-camp-lib/art-camp-01.png" />
    <img src="~/assets/art-camp-lib/art-camp-02.png" />
    <img src="~/assets/art-camp-lib/art-camp-03.png" />
  </article>
</template>
