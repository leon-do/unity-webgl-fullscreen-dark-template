# Unity WebGL Full Width && Dark Theme

![demo](https://user-images.githubusercontent.com/19412160/86728110-1ef01080-bffa-11ea-9966-f9971a05c92d.gif)

## How to use

Create a folder under `/Assets/WebGLTemplates/WebGLTemplates`

Download `FullDarkThemeTemplate` from here and paste under `WebGLTemplates`

![Screen Shot 2020-07-07 at 2 34 38 AM](https://user-images.githubusercontent.com/19412160/86728391-6aa2ba00-bffa-11ea-8430-2a8ab7d5aae5.png)

To use

![Screen Shot 2020-07-07 at 2 25 13 AM](https://user-images.githubusercontent.com/19412160/86728720-b05f8280-bffa-11ea-8532-64d9b1185315.png)

Player Settings...

![Screen Shot 2020-07-07 at 2 25 22 AM](https://user-images.githubusercontent.com/19412160/86728763-bbb2ae00-bffa-11ea-8c00-25298155df97.png)

Update the WebGL Template

![Screen Shot 2020-07-07 at 2 37 17 AM](https://user-images.githubusercontent.com/19412160/86728817-cd945100-bffa-11ea-9e97-3863460578c1.png)

## Under the hood

The base is from the `Default` template.

`style.css` was changed

```css
html {
  background-color: black;
}

/* maintain 960x540 aspect ratio */
#unityContainer {
  width: 100vw;
  height: 56.25vw;
}

@media only screen and (max-width: 960px), (max-height: 540px) {
  #unityContainer {
    width: 960px;
    height: 540px;
  }
}

.webgl-content * {
  border: 0;
  margin: 0;
  padding: 0;
}

.webgl-content {
  position: absolute;
  top: 50%;
  left: 50%;
  -webkit-transform: translate(-50%, -50%);
  transform: translate(-50%, -50%);
}

```

## resources

https://docs.unity3d.com/530/Documentation/Manual/webgl-templates.html
