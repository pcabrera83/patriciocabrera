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

If you are adding them to a component that has MJML as its children (for example, `mj-column` or `mj-section`), 
you need to wrap the handlebars tags in `<mj-raw>` so that aren't swallowed: 

```xml
<!-- This text will repeat for each person -->
<mj-column>
    <mj-raw>{{#each people}}</mj-raw>
        <mj-text>Hi, {{ name }}</mj-text>
    <mj-raw>{{/each}}></mj-raw>
</mj-column>

<!-- DON'T DO THIS - it won't work: -->
<mj-column>
    {{#each people}}
        <mj-text>Hi, {{ name }}</mj-text>
    {{/each}}>
</mj-column>
```


To preview how a template will work with realistic sample data, create a sample data file 
called `templates/[templateName]/sample-data.json` and then preview the template with 
`npm run builder preview [templateName]`