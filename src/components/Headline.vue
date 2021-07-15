  <template>
    <div id="headline">
        <div class="container-fluid p-0">
            <div class="row no-gutters">
                <div class="col-sm-12 col-md-6 row no-gutters" id="headlines">
                    <div class="col-sm-12 col-md-6 bg-body">
                        <div class="tile news-headline-container">
                            <div class="date">
                                <img src="/images/icons/calendar-grey.png" class="mr-2"/>
                                <span class="text-grey">23 mai 2021</span>
                            </div>
                            <div class="news-headline">News headline</div>
                            <p>Lorem Ipsum. Proin gravida nibh velit auctor aliquet. Aenean sollicitudin.</p>
                        </div>
                    </div>
                    <div class="col-sm-12 col-md-6 bg-black">
                        <div class="tile news-headline-container">
                            <div class="date">
                                <img src="/images/icons/calendar-grey.png" class="mr-2"/>
                                <span class="text-grey">23 mai 2021</span>
                            </div>
                            <div class="news-headline">News headline</div>
                            <p class="text-white">Lorem Ipsum. Proin gravida nibh velit auctor aliquet. Aenean sollicitudin.</p>
                        </div>
                    </div>
                </div>
                <div class="col-sm-12 col-md-6">
                    <div class="tile calendar-map" id="image-map-1">
                        <div class="date">17 mai</div>
                        <div class="date-title">headline beitrag 2021</div>
                        <div class="date-subtitle">subtitle</div>
                        <p>Lorem Ipsum. Proin gravida nibh vel velit auctor aliquet. Aenean sollicitudin, lorem quis bibendum auctor.</p>
                    </div>
                </div>
            </div>
            <div class="row no-gutters">
                <div class="col-sm-12 col-md-6">
                    <div class="tile" id="image-boat"></div>
                </div>
                <div class="col-sm-12 col-md-6 row no-gutters">
                    <div class="col-sm-12">
                        <div class="tile calendar-map" id="image-map-2">
                            <div class="date">03 okt</div>
                            <div class="date-title">headline beitrag 2021</div>
                            <div class="date-subtitle">subtitle ort - jahr</div>
                            <p>Lorem Ipsum. Proin gravida nibh vel velit auctor aliquet. Aenean sollicitudin, lorem quis bibendum auctor.</p>
                        </div>
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
                <div class="col-sm-12 col-md-6">
                    <div class="tile tile-black">
                        <img src="/images/icons/newspaper.png" />
                        <div>
                            segelteam<br>
                            termine 2021
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'Headline',
}
</script>