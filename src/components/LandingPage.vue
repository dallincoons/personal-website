<template>
  <div class="page-wrapper">
      <div class="section-wrapper">
          <ul class="list-of-articles">
              <li class="article">
                  <a href="https://medium.com/@dallincoons/the-problem-with-accessors-and-mutators-in-laravel-c1f9a71d7b06" target="_blank">
                      <h4 class="article-title">How to Rapidly Introduce Tests When There Is No Test Coverage.</h4>
                  </a>
                  <p class="article-meta-data">July 19, 2020</p>
                  <p class="article-preview">Introducing test coverage into an existing codebase is a daunting challenge.</p>
              </li>
              <li class="article">
                  <a href="https://medium.com/@dallincoons/the-problem-with-accessors-and-mutators-in-laravel-c1f9a71d7b06" target="_blank">
                      <h4 class="article-title">Ideas For Keeping Your Controllers Skinny</h4>
                  </a>
                  <p class="article-meta-data">May 17, 2020</p>
                  <p class="article-preview">It’s important to keep in mind the responsibility of each class in your system.</p>
              </li>
              <li class="article">
                <a href="https://medium.com/@dallincoons/the-problem-with-accessors-and-mutators-in-laravel-c1f9a71d7b06" target="_blank">
                    <h4 class="article-title">The Problem With Accessors and Mutators In Laravel</h4>
                </a>
                  <p class="article-meta-data">July 21, 2019</p>
                  <p class="article-preview">The Laravel framework feels magical in large part because it heavily uses PHP’s “magic methods” to add many conveniences.</p>
                </li>
              <li class="article">
                <a href="http://dallincoons.github.io/2019/01/20/constructors-in-php-traits.html" target="_blank">
                    <h4 class="article-title">Constructors in Traits</h4>
                </a>
                  <p class="article-meta-data">January 20, 2019</p>
                  <p class="article-preview">Traits are a handy way for sharing functionality in multiple classes, and since php doesn’t support multiple inheritance, this is the next best thing.</p>
              </li>
              <li class="article">
                <a href="http://dallincoons.github.io/2019/01/05/repository-decorators.html" target="_blank">
                    <h4 class="article-title">Using the decorator design pattern with repositories</h4>
                </a>
                    <p class="article-meta-data">January 5, 2019</p>
                    <p class="article-preview">I recently encountered something in the legacy app I’m working in, where the author added caching to at least a dozen or so repositories.</p>
              </li>
              <li class="article">
                <a href="http://dallincoons.github.io/2018/12/30/named-constructors.html" target="_blank">
                    <h4 class="article-title">Named Constructors To Make Our Lives Easier</h4>
                </a>
                    <p class="article-meta-data">December 30, 2018</p>
                    <p class="article-preview">Have you ever found yourself adding parameters with <span class="code">null</span> as defaults in your constructors?</p>
              </li>
              <li class="article">
                <a href="http://dallincoons.github.io/2018/12/22/dont-mock-what-you-dont-own-example.html" target="_blank">
                    <h4 class="article-title">Don't Mock What You Don't Own</h4>
                </a>
                    <p class="article-meta-data">December 22, 2018</p>
                    <p class="article-preview">The maxim “Don’t Mock What You Don’t Own” was cryptic to me when I first heard it. Even searching the internet for clues wasn’t much help. </p>
              </li>
              <li class="article">
                <a href="http://dallincoons.github.io/2018/10/24/managing-software-projects.html" target="_blank">
                    <h4 class="article-title">Managing Software Projects</h4>
                </a>
                    <p class="article-meta-data">October 24, 2018</p>
                    <p class="article-preview">Have you ever pushed through bad code in the name of a deadline? It’s ok, we all have, which is the reality of life. </p>
              </li>
              <li class="article">
                <a href="http://dallincoons.github.io/2018/10/10/repository-test-doubles.html" target="_blank">
                    <h4 class="article-title">My favorite reason to use the repository pattern</h4>
                </a>
                    <p class="article-meta-data">October 10, 2018</p>
                    <p class="article-preview">Not everyone is in love with the Repository Pattern, which is understandable, because it has a way of complicating things and adding a lot of seemingly unneccessary code, especially in small, Active Record style apps.</p>
              </li>
          </ul>
      </div>

  </div>
</template>

<script>
export default {
  name: 'LandingPage',
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

.section-title {
    text-transform: uppercase;
    color: #0D0D0D;
    font-size: 1.5rem;
    margin-bottom: .5rem;
    grid-column: 1 / span 5;
}

.section-wrapper {
    margin-top: 3rem;
    display: grid;
    grid-template-columns: repeat(5, 1fr);
    grid-template-rows: 1fr auto;
    grid-gap: 20px;
}

.project {
    border: 2px solid #01ABD1;
    border-bottom: 8px solid #01abd1;
    padding: .5rem;
    margin-bottom: 2rem;
    display: flex;
    flex-direction: column;
    justify-content: space-between;
    cursor: pointer;
    position: relative;
    grid-column: auto / span 2;
}


.project-title {
    margin: 0;
    font-size: 1.2rem;
}

.project-description {
    line-height: 2;
}

.project-details {
    z-index: 0;
}

.project:hover .project-more {
    height: 75px;
    opacity: 1;
    background: rgba(16,171,209,.65);
    transition: all .4s ease-in-out;
}

.project-more {
    background: rgba(16,171,209,0);
    position: absolute;
    bottom: 0;
    opacity: 0;
    height: 0;
    width: 100%;
    color: #0d0d0d;
    margin: -.5rem;
    display: grid;
    justify-items: center;
    align-items: center;
    font-weight: 600;
    font-size: 1.2rem;
    text-decoration: none;
    transition: all .4s ease-in-out;
}


.list-of-articles {
    grid-column: 1 / span 3;
}

.article {
    margin: 2rem 0 5rem 0;
    /*text-transform: capitalize;*/
}

.article a {
    text-decoration: none;
    /*color: #01ABD1;*/
    color: #0d0d0d;
    transition: all .2s ease-in-out;
}

.article:hover a {
    font-weight: 700;
    color: #01ABD1;
    transition: all .2s ease-in-out;
}
.article-title {
    font-weight: 700;
    font-size: 2rem;
    margin-bottom: .5rem;
}

.article-meta-data {
    color: #01ABD1;
    margin: 0;
}


.article-preview {
    /*font-family: 'Crimson Pro', serif;*/
    /*font-size: 1.2rem;*/
    margin-top: .5rem;
}

.code {
    font-family: 'Roboto Mono', monospace;
}


@media (max-width: 900px) {

    .section-wrapper {
        grid-template-columns: 1fr;
    }

    .section-title {
        grid-column: 1;
    }

    .project-more {
        height: 56px;
        opacity: 1;
    }

}



</style>
