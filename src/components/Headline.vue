  <template>
    <div id="headline">
        <div class="container-fluid p-0">
            <div class="row no-gutters">
                <div class="col-sm-12 col-md-6 row no-gutters" id="headlines">
                    <div class="col-sm-12 col-md-6 bg-body">
                        <div class="tile news-headline-container">
                            <div class="cursor-pointer" @click="openNews()">
                                <div class="date">
                                    <img src="/images/icons/calendar-grey.png" class="mr-2"/>
                                    <span class="text-grey">23 mai 2021</span>
                                </div>
                                <div class="news-headline">News headline</div>
                                <p>Lorem Ipsum. Proin gravida nibh velit auctor aliquet. Aenean sollicitudin.</p>
                            </div>
                        </div>
                    </div>
                    <div class="col-sm-12 col-md-6 bg-black">
                        <div class="tile news-headline-container">
                            <div class="cursor-pointer" @click="openNews()">
                                <div class="date">
                                    <img src="/images/icons/calendar-grey.png" class="mr-2"/>
                                    <span class="text-grey">23 mai 2021</span>
                                </div>
                                <div class="news-headline">News headline</div>
                                <p class="text-white">Lorem Ipsum. Proin gravida nibh velit auctor aliquet. Aenean sollicitudin.</p>
                            </div>
                        </div>
                    </div>
                </div>
                <div class="col-sm-12 col-md-6">
                    <a href="#" class="tile calendar-map" id="image-map-1">
                        <div class="date">17 mai</div>
                        <div class="date-title">headline beitrag 2021</div>
                        <div class="date-subtitle">subtitle</div>
                        <p>Lorem Ipsum. Proin gravida nibh vel velit auctor aliquet. Aenean sollicitudin, lorem quis bibendum auctor.</p>
                    </a>
                </div>
            </div>
            <div class="row no-gutters">
                <div class="col-sm-12 col-md-6">
                    <div class="tile" id="image-boat"></div>
                </div>
                <div class="col-sm-12 col-md-6 row no-gutters">
                    <div class="col-sm-12">
                        <a  href="#" class="tile calendar-map" id="image-map-2">
                            <div class="date">03 okt</div>
                            <div class="date-title">headline beitrag 2021</div>
                            <div class="date-subtitle">subtitle ort - jahr</div>
                            <p>Lorem Ipsum. Proin gravida nibh vel velit auctor aliquet. Aenean sollicitudin, lorem quis bibendum auctor.</p>
                        </a>
                    </div>
                    <div class="col-sm-12 col-md-6">
                        <div class="tile" id="image-flag"></div>
                    </div>
                    <div class="col-sm-12 col-md-6">
                        <div class="tile" id="image-boat-small"></div>
                    </div>
                </div>
            </div>
            <div class="row no-gutters">
                <div class="col-sm-12 col-md-6">
                    <div class="tile tile-black" id="news-bilder">
                        <img src="/images/icons/newspaper.png" class="text-center" />
                        <div>
                            news+<br>
                            bilder
                        </div>
                    </div>
                </div>
                <div href="#" class="col-sm-12 col-md-6">
                    <a href="#" class="tile tile-black">
                        <img src="/images/icons/newspaper.png" />
                        <div>
                            segelteam<br>
                            termine 2021
                        </div>
                    </a>
                </div>
            </div>
        </div>
        <div id="news-overlay-body" :class="{'opened': newsOpened}">
            <div>
                <div class="bg-white p-5">
                    <div class="d-flex align-items-baseline mb-4">
                        <img src="/images/icons/calendar-grey.png" class="mr-2"><b class=text-grey>23. MAI 2021</b>
                    </div>
                    <div class="row">
                        <div class="col col-md-6">
                            <h1>
                                NEWSARTIKEL <br>
                                HEADLINE
                            </h1>
                            <h4 class="mb-4">Lorem Ipsum Proin gravida nibh vel velit</h4>
                            <div class="divider"></div>
                            <p>Lorem Ipsum. Proin gravida nibh vel velit auctor aliquet. Aenean sollicitudin, lorem quis bibendum auctor, nisi elit consequat ipsum, nec sagittis sem nibh id elit. Duis sed odio sit amet nibh vulputate cursus a sit amet mauris. Morbi accumsan ipsum velit. Nam nec tellus a odio tincidunt auctor a ornare odio. Sed non  mauris vitae erat consequat auctor eu in elit. Class aptent taciti sociosqu ad litora torquent per conubia nostra, per inceptos himenaeos. Mauris in erat justo. Nullam ac urna eu felis dapibus condimentum sit amet a augue. Sed non neque elit. Sed ut imperdiet nisi. Proin condimentum fermentum nunc. Etiam pharetra, erat sed fermentum feugiat, velit mauris egestas quam, ut aliquam massa nisl quis neque. Suspendisse in orci enim.</p>
                            <p>Lorem Ipsum. Proin gravida nibh vel velit auctor aliquet. Aenean sollicitudin, lorem quis bibendum auctor, nisi elit consequat psum, nec sagittis sem nibh id elit. Duis sed odio sit amet nibh vulputate cursus a sit amet mauris. Morbi accumsan ipsum velit. Nam nec tellus a odio tincidunt auctor a ornare odio. Sed non  mauris vitae erat consequat auctor eu in elit. Class aptent taciti sociosqu ad litora torquent per conubia nostra, per inceptos himenaeos. Mauris in erat justo. Nullam ac urna eu felis dapibus condimentum sit amet a augue. Sed non neque elit. Sed ut imperdiet nisi. Proin condimentum fermentum nunc. Etiam pharetra, erat sed fermentum feugiat, velit mauris egestas quam, ut aliquam massa nisl quis neque. Suspendisse in orci enim. Lorem Ipsum. Proin gravida nibh vel velit auctor aliquet. Aenean sollicitudin, lorem quis bibendum auctor, nisi elit consequat ipsum, nec sagittis sem nibh id elit.</p>
                            <p>Duis sed odio sit amet nibh vulputate cursus a sit amet mauris. Morbi accumsan ipsum velit. Nam nec tellus a odio tincidunt auctor a ornare odio. Sed non  mauris vitae erat consequat auctor eu in elit.</p>
                        </div>
                        <div class="col col-md-6">
                            <div id="news-images-gallery">
                                <div class="gallery-navigation left">
                                    <img src="/images/icons/arrow-left.png"/>
                                </div>
                                <img src="/images/news-main-image.jpg" alt="The team" class="gallery-image"/>
                                <span id="gallery-counter">1/10</span>
                                <div class="gallery-navigation right">
                                    <img src="/images/icons/arrow-right.png"/>
                                </div>
                            </div>
                            <p>Lorem Ipsum. Proin gravida nibh vel velit auctor aliquet. Aenean sollicitudin, lorem quis bibendum auctor, nisi elit consequat ipsum, nec sagittis sem nibh id elit. Duis sed odio sit amet nibh vulputate cursus a sit amet mauris. Morbi accumsan ipsum velit. Nam nec tellus a odio tincidunt auctor a ornare odio. Sed non  mauris vitae erat consequat auctor eu in elit. Class aptent taciti sociosqu ad litora torquent per conubia nostra, per inceptos himenaeos. Mauris in erat justo. Nullam ac urna eu felis dapibus condimentum sit amet a augue. Sed non neque elit. Sed ut imperdiet nisi. Proin condimentum fermentum nunc. Etiam pharetra, erat sed fermentum feugiat, velit mauris egestas quam, ut aliquam massa nisl quis neque. Suspendisse in orci enim. Lorem Ipsum. Proin gravida nibh vel velit auctor aliquet. Aenean sollicitudin, lorem quis bibendum auctor, nisi elit consequat ipsum, nec sagittis sem nibh id elit. Duis sed odio sit amet nibh vulputate cursus a sit amet mauris. Morbi accumsan ipsum velit. Nam nec tellus a odio tincidunt auctor a ornare odio. Sed non  mauris vitae erat consequat auctor eu in elit. Class aptent taciti sociosqu ad litora torquent per conubia nostr.</p>
                        </div>
                    </div>
                </div>
                <div class="bg-body p-5">
                    <div id="other-articles-subtitle">Ältere Artikel</div>
                    <div id="other-articles">
                        <div class="article-navigation left">
                            <img src="/images/icons/arrow-left-black.png"/>
                        </div>
                        <div id="other-articles-body" class="row">
                            <div class="col-sm-12 col-md-3 article">
                                <img src="/images/news-image-1.jpg"/>
                                <div clasS="article-headline">Headline von einem  älteren Artikel</div>
                                <div>Lorem Ipsum. Proin gravida nibh vel velit auctor aliquet. Aenean sollicitudin, lorem quis bibendum auctor, nisi elit consequat ipsum, nec sagittis sem nibh id elit. Duis sed odio sit amet nibh vulputate cursus a sit amet mauris. Morbi accumsan ipsum velit.</div>
                            </div>
                            <div class="col-sm-12 col-md-3 article">
                                <img src="/images/news-image-2.jpg"/>
                                <div clasS="article-headline">Headline von einem  älteren Artikel</div>
                                <div>Lorem Ipsum. Proin gravida nibh vel velit auctor aliquet. Aenean sollicitudin, lorem quis bibendum auctor, nisi elit consequat ipsum, nec sagittis sem nibh id elit. Duis sed odio sit amet nibh vulputate cursus a sit amet mauris. Morbi accumsan ipsum velit.</div>
                            </div>
                            <div class="col-sm-12 col-md-3 article">
                                <img src="/images/news-image-3.jpg"/>
                                <div clasS="article-headline">Headline von einem  älteren Artikel</div>
                                <div>Lorem Ipsum. Proin gravida nibh vel velit auctor aliquet. Aenean sollicitudin, lorem quis bibendum auctor, nisi elit consequat ipsum, nec sagittis sem nibh id elit. Duis sed odio sit amet nibh vulputate cursus a sit amet mauris. Morbi accumsan ipsum velit.</div>
                            </div>
                            <div class="col-sm-12 col-md-3 article">
                                <img src="/images/news-image-4.jpg"/>
                                <div clasS="article-headline">Headline von einem  älteren Artikel</div>
                                <div>Lorem Ipsum. Proin gravida nibh vel velit auctor aliquet. Aenean sollicitudin, lorem quis bibendum auctor, nisi elit consequat ipsum, nec sagittis sem nibh id elit. Duis sed odio sit amet nibh vulputate cursus a sit amet mauris. Morbi accumsan ipsum velit.</div>
                            </div>
                        </div>
                        <div class="article-navigation right">
                            <img src="/images/icons/arrow-right-black.png"/>
                        </div>
                    </div>
                </div>
            </div>
            <div id="overlay-icons">
                <div class="overlay-icon bg-body" @click="closeNews()">
                    <img src="/images/icons/icon-close.png" />
                </div>
                <div class="overlay-icon bg-black">
                    <img src="/images/icons/facebook-white.png" />
                </div>
                <div class="overlay-icon bg-black">
                    <img src="/images/icons/twitter-white.png" />
                </div>
                <div class="overlay-icon bg-black">
                    <img src="/images/icons/googleplus-white.png" />
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'Headline',
     data(){
        return{
            newsOpened: false,
        }
    },
    methods: {
        openNews() {
            this.newsOpened = true
            document.getElementById('popup-backdrop').classList.add('opened')
        },
        closeNews() {
            this.newsOpened = false
            document.getElementById('popup-backdrop').classList.remove('opened')
        }
    },
    mounted() {}
}
</script>