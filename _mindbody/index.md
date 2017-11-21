---
#
---
<html>
    <head>
        <meta charset="utf-8">
        <meta http-equiv="x-ua-compatible" content="ie=edge">
        <meta name='viewport' content='width=device-width, initial-scale=1, shrink-to-fit=no'/>
        
        <title>{{ site.title | default: site.github.repository_name }} by {{ site.github.owner_name }}</title>

        {% include mindbody/stylesheets.html %}
    </head>
    <body>
        <header>
            {% include mindbody/header-nav.html %}
        </header>
        <div class='w-100 bg-dark d-flex align-items-center justify-content-center border text-white' style='min-height:30vh'> 
            <h1 class="d-inline-block text-truncate display-4" style="max-width:80vw;">
  Praeterea iter est quasdam res quas ex communi.</h1>
        </div>

        <div class="container card border-0 rounded bg-white w-75" style='margin-top:-5vh; min-height:75vh; box-shadow: 5px 5px 10px rgba(0, 0, 0, 0.175);'>
            <section class='container'>
                <div class='row'>
                    <div class='text-center mx-auto col-md-10 m-3'>
                    <p>
                    Lorem ipsum dolor sit amet, consectetur adipiscing elit. Integer posuere erat a ante. Lorem ipsum dolor sit amet, consectetur adipiscing elit. Integer posuere erat a ante. Lorem ipsum dolor sit amet, consectetur adipiscing elit. Integer posuere erat a ante.
                    </p>
                    </div>
                </div>
            </section>
        </div>

        <div class='w-100 bg-dark d-flex align-items-center justify-content-center border text-white' style='min-height:20vh; margin-top:-2vh;'>
            <section>
                        <div class='text-center'>
                            <img class="rounded-circle mt-3" src="https://placehold.it/96x96" />
                                <p class='m-1 col-md-12'><small>
                                Lorem ipsum dolor sit amet, consectetur adipiscing elit. Integer posuere erat a ante. Lorem ipsum dolor sit amet, consectetur adipiscing elit. Integer posuere erat a ante. Lorem ipsum dolor sit amet, consectetur adipiscing elit. Integer posuere erat a ante.
                            </small></p>
                        </div>
            </section>
        </div>

        {% include footer.html %}

        <!-- JavaScript: placed at the end of the document so the pages load faster -->
        {% include scripts.html %}
    </body>
</html>