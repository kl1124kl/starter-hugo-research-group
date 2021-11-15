{{ define "main" }}
<main class="bg-white min-vh-100">
  <article class="container mb-5">
    <div class="row gx-lg-5">

      <!--      Header section (in narrow screens) - Left Column (in wide screens 'lg')      -->
      <div class="col-12 col-lg-6 pt-5 sticky-lg-top h-100">
        <!--    Title     -->
        <h1 class="mb-4 mb-md-5 text-center fw-light text-uppercase">{{ .Title | safeHTML }}</h1>
          {{- $imageWebp := .Resources.GetMatch "*feature*.webp" }}
          {{- $imageJpg := .Resources.GetMatch "*feature*.jp*" }}
          {{- $path := path.Join "content" $imageWebp.RelPermalink }}
          {{- $imgAttributes := imageConfig $path }}
        <!--    Featured image     -->
        <picture>
          <source srcset="{{ $imageWebp.RelPermalink }}" type="image/webp">
          <img 
            src="{{ $imageJpg.RelPermalink }}" 
            alt='{{ print "Imagen principal: " $imageWebp.Name }}' 
            width="{{ $imageJpg.Width }}" 
            height="{{ $imageJpg.Height }}">
        </picture>
        <p class="my-4 small text-muted">
          {{ .Page.Description | safeHTML }}
          <!-- It can also just be: {{ .Description }} -->
        </p>

        <!--    Button for ToC - Wide screens      -->
        {{ if .Params.Toc }}
          <div class="d-none d-lg-flex justify-content-end">
            <button class="btn btn-outline-primary" type="button" data-bs-toggle="offcanvas" data-bs-target="#offcanvasToc" aria-controls="offcanvasToc">
              {{ T "table_of_content" }}
            </button>
          </div>
        {{ end }}
      </div>

      <!--      Content section (in narrow screens) - Right Column (in wide screens 'lg')            -->
      <div class="col-12 col-lg-6 py-lg-5">
        <!--    Icons -->
        {{ with .Param "icon" }}
          <p class="fs-1 text-center text-gris-claro">
            {{ . }}
          </p>          
        {{ end }}
        {{ if .Params.Toc }}
        <!--    Table of Contents in Accordion - Narrow screens -->
          <nav class="accordion d-lg-none lh-lg mb-5" id="accordionToc">
            <div class="accordion-item">
              <h2 class="accordion-header mt-0" id="accordionTocHeading">
                <button class="accordion-button collapsed fs-4 fw-light" type="button" data-bs-toggle="collapse" data-bs-target="#accordionTocBody" aria-expanded="false" aria-controls="accordionTocBody">
                  {{ T "table_of_content" | upper }}
                </button>
              </h2>
              <div class="accordion-collapse collapse" id="accordionTocBody" aria-labelledby="accordionTocHeading" data-bs-parent="#accordionToc">
                <div class="accordion-body">
                  {{ .TableOfContents }}
                </div>
              </div>
            </div>
          </nav>
        {{ end }}

        <!--    Markdown content    -->
        {{ .Content }}


        <!--    Sharing buttons     -->
        <aside class="text-end">
          {{ partial "share-buttons.html" . }}
        </aside>

        <!--    Related Tips        -->
        <aside class="list-group list-group-flush">
          <h2 class="mt-5">
            Más Tips útiles...
          </h2>
          {{ $related := .Site.RegularPages.Related . | first 4 }}
          {{ with $related }}
            {{ range $related }}
              <a class="list-group-item list-group-item-action px-2 mt-3" href="{{ .RelPermalink }}">
                {{ partial "page-snippet-related.html" . }}
              </a>
            {{ end }}
          {{ end }}
        </aside>

      </div>
    </div>
  </article>

  <!--          Table of Contents - For wide screens    -->
  <!--          It is activated with the button for ToC. See above. -->
  <nav>
    <!-- bootstrap - offcanvas   -->
    <div class="offcanvas offcanvas-start" tabindex="-1" id="offcanvasToc" data-bs-scroll="true" aria-labelledby="offcanvasTocLabel">
      <!-- offcanvas header   -->
      <div class="offcanvas-header">
        <h1 class="text-uppercase fw-light text-primary fs-3 ps-2" id="offcanvasTocLabel">{{ T "table_of_content" }}</h1>
        <button type="button" class="btn-close text-reset" data-bs-dismiss="offcanvas" aria-label="Close"></button>
      </div>
      <!-- offcanvas body    -->
      <div class="offcanvas-body lh-lg">
        {{.TableOfContents}}
      </div>
    </div>
  </nav>
</main>
{{ end }}
