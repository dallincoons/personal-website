<template>
  <div class="page-wrapper">
    <div class="section-wrapper">
        <h3 class="section-title">Projects</h3>
        <div class="project">
            <div>
                <h4 class="project-title">Pepper Rodeo</h4>
                <p class="project-description">
                    The sky calls to us invent the universe a very small stage in a vast cosmic arena another world another world descended from astronomers and billions upon billions upon billions upon billions upon billions upon billions upon billions.
                </p>
            </div>
            <router-link class="project-more" to="/pepper-rodeo">More Info</router-link>
        </div>
        <div class="project ">
            <div>
                <h4 class="project-title">Brainframe Recall</h4>
                <p class="project-description">
                    Hearts of the stars Sea of Tranquility galaxies from which we spring billions upon billions Cambrian explosion.
                </p>
            </div>
            <a class="project-more">More Info</a>
        </div>
        <div class="project ">
            <div>
                <h4 class="project-title">Alfred.fm</h4>
                <p class="project-description">
                    Hearts of the stars Sea of Tranquility galaxies from which we spring billions upon billions Cambrian explosion.
                </p>
            </div>
            <a class="project-more">More Info</a>
        </div>
        <div class="project ">
            <div>
                <h4 class="project-title">Politician Tweet Generator</h4>
                <p class="project-description">
                    Hearts of the stars Sea of Tranquility galaxies from which we spring billions upon billions Cambrian explosion.
                </p>
            </div>
            <a class="project-more">More Info</a>
        </div>
        <div class="project ">
            <div>
                <h4 class="project-title">Spotify Preferences</h4>
                <p class="project-description">
                    Hearts of the stars Sea of Tranquility galaxies from which we spring billions upon billions Cambrian explosion.
                </p>
            </div>
            <a class="project-more">More Info</a>
        </div>
    </div>
    <div class="section-wrapper">
        <h3 class="section-title">Articles</h3>
        <ul class="list-of-articles">
            <li class="article"><a href="https://medium.com/@dallincoons/the-problem-with-accessors-and-mutators-in-laravel-c1f9a71d7b06" target="_blank">The Problem With Accessors and Mutators In Laravel</a></li>
            <li class="article"><a href="http://dallincoons.github.io/2019/01/20/constructors-in-php-traits.html" target="_blank">Constructors in Traits</a></li>
            <li class="article"><a href="http://dallincoons.github.io/2019/01/05/repository-decorators.html" target="_blank">Using the decorator design pattern with repositories</a></li>
            <li class="article"><a href="http://dallincoons.github.io/2018/12/30/named-constructors.html" target="_blank">Named Constructors To Make Our Lives Easier</a></li>
            <li class="article"><a href="http://dallincoons.github.io/2018/12/22/dont-mock-what-you-dont-own-example.html" target="_blank">Don't Mock What You Don't Own</a></li>
            <li class="article"><a href="http://dallincoons.github.io/2018/10/24/managing-software-projects.html" target="_blank">Managing Software Projects</a></li>
            <li class="article"><a href="http://dallincoons.github.io/2018/10/10/repository-test-doubles.html" target="_blank">My favorite reason to use the repository pattern</a></li>
            <li class="article"><a href="http://dallincoons.github.io/2016/06/30/min-height-inheritance.html" target="_blank">CSS - Min height inheritance</a></li>
            <li class="article"><a href="http://dallincoons.github.io/2016/06/01/Cache-factory-service.html" target="_blank">Cache Factory service</a></li>
            <li class="article"><a href="http://dallincoons.github.io/2016/05/27/Angular-pre-and-post-links.html" target="_blank">Angular Pre and Post links</a></li>
            <li class="article"><a href="http://dallincoons.github.io/2016/05/27/Angular-adventures-with-providers.html" target="_blank">Adventures with providers</a></li>
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
    grid-column: 1 / span 3;
}

.section-wrapper {
    margin-top: 3rem;
    display: grid;
    grid-template-columns: repeat(3, 1fr);
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
}


.project-title {
    margin: 0;
    font-size: 1.2rem;
}

.project-description {
    line-height: 2;
}

.project:hover .project-more {
    height: 56px;
    opacity: 1;
    transition: all .4s ease-in-out;
}

.project-more {
    background: #10abd1;
    opacity: 0;
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
    margin-bottom: 1rem;
    text-transform: capitalize;
}

.article a {
    text-decoration: none;
    color: #01ABD1;
    font-weight: 500;
    transition: all .2s ease-in-out;
}

.article:hover a {
    font-weight: 700;
    color: #0d0d0d;
    transition: all .2s ease-in-out;
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
