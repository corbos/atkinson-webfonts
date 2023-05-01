# Atkinson Hyperlegible Font Example

1. Download the Atkinson Hyperlegible Font zip.

2. Unzip.

3. Copy the `Web Fonts` directory into a project. (Possibly rename it without a space.)

4. Create a stylesheet and add a `@font-face` at-rule. Use an appropriate relative path.

    ```css
    @font-face {
        font-family: "Atkinson-Hyperlegible-Regular";
        src: local("Atkinson-Hyperlegible-Regular"),
        url("../webfonts/eot/Atkinson-Hyperlegible-Regular-102.eot") format("embedded-opentype"),
        url("../webfonts/eot/Atkinson-Hyperlegible-Regular-102.eot"),
        url("../webfonts/woff2/Atkinson-Hyperlegible-Regular-102a.woff2") format("woff2"),
        url("../webfonts/woff/Atkinson-Hyperlegible-Regular-102.woff") format("woff"),
        url("../webfonts/ttf/Atkinson-Hyperlegible-Regular-102.ttf") format("truetype"),
        url("../webfonts/svg/Atkinson-Hyperlegible-Regular-102.svg") format("svg");
        font-weight: normal;
        font-size: normal;
    }
    ```

    Here's a strategy for particular font types: https://developer.mozilla.org/en-US/docs/Web/CSS/@font-face/src#fallbacks_for_older_browsers

5. Use the `font-family` where ever.

    ```css
    h1 {
        font-family: "Atkinson-Hyperlegible-Regular", sans-serif;
    }

    .hyperlegible {
        font-family: "Atkinson-Hyperlegible-Regular", sans-serif;
    }
    ```