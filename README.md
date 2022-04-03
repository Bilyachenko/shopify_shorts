# shopify_shorts
shopify shorts codes

<h4>Create shopify section:</h4>
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
