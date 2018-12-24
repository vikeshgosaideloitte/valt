# Hello Abi 

Here's your final Christmas present! 

<div class='tableauPlaceholder' id='viz1545619772641' style='position: relative'><noscript><a href='#'><img alt=' ' src='https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;VA&#47;VALT&#47;Dashboard1&#47;1_rss.png' style='border: none' /></a></noscript><object class='tableauViz'  style='display:none;'><param name='host_url' value='https%3A%2F%2Fpublic.tableau.com%2F' /> <param name='embed_code_version' value='3' /> <param name='site_root' value='' /><param name='name' value='VALT&#47;Dashboard1' /><param name='tabs' value='no' /><param name='toolbar' value='yes' /><param name='static_image' value='https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;VA&#47;VALT&#47;Dashboard1&#47;1.png' /> <param name='animate_transition' value='yes' /><param name='display_static_image' value='yes' /><param name='display_spinner' value='yes' /><param name='display_overlay' value='yes' /><param name='display_count' value='yes' /></object></div>                <script type='text/javascript'>                    var divElement = document.getElementById('viz1545619772641');                    var vizElement = divElement.getElementsByTagName('object')[0];                    vizElement.style.minWidth='420px';vizElement.style.maxWidth='650px';vizElement.style.width='100%';vizElement.style.minHeight='587px';vizElement.style.maxHeight='887px';vizElement.style.height=(divElement.offsetWidth*0.75)+'px';                    var scriptElement = document.createElement('script');                    scriptElement.src = 'https://public.tableau.com/javascripts/api/viz_v1.js';                    vizElement.parentNode.insertBefore(scriptElement, vizElement);                </script>


<html>
<head>
<script src="https://code.jquery.com/jquery-2.1.1.min.js"></script>
  </script>
  <script>    
    
    function swapImages(){
      var $active = $('#myGallery .active');
      var $next = ($('#myGallery .active').next().length > 0) ? $('#myGallery .active').next() : $('#myGallery img:first');

      $next.fadeIn(function(){         
        $active.removeClass('active');
        $next.addClass('active');
        $active.fadeOut();
      })
            
    }

    $(document).ready(function(){
      
      var height = $( window ).height();
      var width = $( window ).width();
      var size = width + ',' + height;
      
      var locations = [        
        /*** EDIT THIS SECTION ***
 
        Put the links to your viz here, make sure to include the following url parameters
        &:embed=yes&:toolbar=no&:format=png&<filter/parameter>=<value>
        to make sure it auto sizes add this to the url as well &:size="+size+"

        Example:
      
        {"src": "https://public.tableau.com/profile/vik8873#!/vizhome/VALT/Dashboard1?publish=yes"},  

        ** with add'l years **

        {"src": "https://public.tableau.com/profile/vik8873#!/vizhome/VALT/Dashboard1?publish=yes"},
        {"src": "https://public.tableau.com/profile/vik8873#!/vizhome/VALT/Dashboard1?publish=yes"},
        {"src": "https://public.tableau.com/profile/vik8873#!/vizhome/VALT/Dashboard1?publish=yes"},

        */
        {"src": ""},
        
                ]
            
      $("#myGallery").attr('width',width);
      $("#myGallery").attr('height',height);
      
      var img = '';
      
      locations.forEach(function(element, index, array){
        
        
        if(index==0){         
          img = '<img src="'+locations[index].src+'" class="active" />';
        } else {
          img = '<img src="'+locations[index].src+'" />';         
        }

        console.log('index: '+index+' == '+img);    
        
        $(img).appendTo("#myGallery");
        
      })
      
      
      // Change 3000 to whatever time interval you prefer
      setInterval('swapImages()', 3000);
    });
  </script>
  <style>
    
    body {
      background-color: #353535;
    }
    #myGallery{
      position:relative;
    }
    #myGallery img{
      display:none;
      position:absolute;
      top:0;
      left:0;
    }
    #myGallery img.active{
      display:block;
    }
  </style>
</head>
<body>
  <div id="myGallery">
  </div>
</body>
</html>


You can use the [editor on GitHub](https://github.com/vikeshgosaideloitte/valt/edit/master/README.md) to maintain and preview the content for your website in Markdown files.

Whenever you commit to this repository, GitHub Pages will run [Jekyll](https://jekyllrb.com/) to rebuild the pages in your site, from the content in your Markdown files.

### Markdown

Markdown is a lightweight and easy-to-use syntax for styling your writing. It includes conventions for

```markdown
Syntax highlighted code block

# Header 1
## Header 2
### Header 3

- Bulleted
- List

1. Numbered
2. List

**Bold** and _Italic_ and `Code` text

[Link](url) and ![Image](src)
```
