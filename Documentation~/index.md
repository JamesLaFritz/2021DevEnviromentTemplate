---
_tocRel: Manual/toc.html
---

[!include[Read Me](../docs/README.md)]

# Add API documentation
Add this to the doc.json file

```cs
{
  "metadata": [
    {
      "src": [
        {              
          "src":"../",
          "files": ["**.cs"],
          "exclude": [
            "docs/**",
            "**/bin/**",
            "**/obj/**",
			"Documentation~/**",
			".git/**"
          ]
        }
      ],
      "dest": "api",
      "disableGitFeatures": false,
      "disableDefaultFilter": false,
      "force": true
    }
  ],
  "build": {
    "content": [
      {
        "files": ["api/**"]
      },
  }
}

```
