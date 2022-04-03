# shopify_shorts
shopify shorts codes

<h4>Create shopify section exemple:</h4>

<div class="newvidesloder">
	{% for block in section.blocks %}
		<div class="videslide-item">
			<div class="slideitem-video">
				<video autoplay muted loop id="myVideo">
				  <source src="{{ block.settings.videolink }}" type="video/mp4">
				</video>
			</div>
			<div class="slidetextinner">
				<div class="slideinnerfllex">
					<div class="slidetitle">
						{{ block.settings.slidename }}
					</div>
					<div class="slidebtn">
						<a href="{{ block.settings.slidelink }}" class="btn btnwhite">Shop Now</a>
					</div>
				</div>
			</div>
		</div>
	{% endfor %}	
</div>
<hr>
<pre>
  {% schema %}
    {
      "name": "Video Slide 2",
      "max_blocks": 9,
       "settings": [
        {
          "type": "text",
          "id": "heading",
          "default": "Title slide",
          "label": "Heading"
        }
      ],
      "blocks": [
      {
        "type": "image",
        "name": "Image",
        "settings": [
        {
          "id": "slideimage",
          "type": "image_picker",
          "label": "Slide Image"
        },
        {
          "id": "videolink",
          "type": "text",
          "label": "Slide url video"
        },
        {
          "type": "text",
          "id": "slidename",
          "label": "Name"
        },
        {
          "type": "text",
          "id": "slidelink",
          "label": "Link"
        }
        ]
      }
      ],
      "presets": [
        {
          "name": "Video Slide 2"
        }
      ]
    }
  {% endschema %}</pre>
<h4>Create shopify section:</h4>
<pre>
