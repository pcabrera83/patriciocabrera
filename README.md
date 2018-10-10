# Jekyll Static Site Generator

## Format and organization ##

* Each project file has its own file in the `root` directory and ends with `.md`. For example, the `billing-app.md` page is in the `root`.
* The pages start with front matter followed by HTML code and can contain variables  which on compile will be replace with data. 
    * Reusable components can be found in `_includes/*.html` and included like this:
      `{% include footer.html %} `

## Installation ##

1. Check out this repo
2. gem install jekyll bundler
3. jekyll new `<projectName>`
3. Start working!  
4. Compile your project `bundle exec jekyll serve`.  

## Variable substitution ##

Use handlebars-style tags to dynamically include substitution variables.  For example:

```xml
    <a href="{{ site.baseurl }}/">
        Text Link
    </a>
```

If you want to loop through a list you need to create a `<fileName>.YML` in the `_data` folder.

```xml
<!-- Data File _data/project.yml -->
- class: css class
  imgSrc: <imagePath>
  imgAlt: Image Alt Tag
  url: <link>
  Title: Project Title
  Description: 'Project Description'

<!-- Markdown -->
{% for project in site.data.project %}
<div class="work-item {{ project.class }}">
    <div class="work-detail">
        <a href="{{ project.url | relative_url }}">
            <img alt="{{ project.imgAlt }}" src="{{ project.imgSrc | relative_url }}">
            <div class="work-info">
                <div class="centrize">
                    <div class="v-center">
                        <h3>{{ project.title }}</h3>
                        <p>{{ project.description }}</p>
                    </div>
                </div>
            </div>
        </a>
    </div>
</div>
{% endfor %}