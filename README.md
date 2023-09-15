# ejemplo-hugo
Ejemplo de web con Hugo para clase de DAW



## Debug on codespaces

* Open the remote explorer sidebar in Codespaces.
* Forward port 1313
* Right click on entry and copy the url

Run the server command with copied url
```bash
hugo server -D --baseUrl "https://{githubUrl}" --appendPort=false
```

Revisar https://hugo.md/post/editing-in-github-codespaces/
