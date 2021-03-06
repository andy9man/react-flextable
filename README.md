# React Flex Table

[![Build Stats](https://img.shields.io/badge/build-passing-brightgreen.svg)](https://nixtus.com)
[![dependencies Status](https://david-dm.org/nixtus/react-flextable/status.svg)](https://david-dm.org/nixtus/react-flextable)
[![devDependencies Status](https://david-dm.org/nixtus/react-flextable/dev-status.svg)](https://david-dm.org/nixtus/react-flextable?type=dev)
[![peerDependencies Status](https://david-dm.org/nixtus/react-flextable/peer-status.svg)](https://david-dm.org/nixtus/react-flextable?type=peer)
[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)


# Features
* **ES6/ESNext** - Write _ES6_ code and _Babel_ will transpile it to ES5 for backwards compatibility
* **Test** - _Jest_
* **Lint** - Preconfigured _ESlint_ with _Airbnb_ config
* **Minify** - Built code will be not be minified, this allows for easier testability in your application.  Make sure to minify your application for best performance.
* **Styled Components** - Built using styled components with flexibility to allow you to customize them to meet your needs.  Just pass styles and classes as normal props.
* **React Hooks** - Built using react hooks.


# Components
- `<FlexTable>` - Outer table container
- `<FlexHeader>` - Acts like a row but removes row clickable events and adds header styling by default
- `<FlexFooter>` - Acts like a row but removes row clickable events
- `<FlexRow>` -  Table Row container
- `<FlexItem>` - Table item container
- `<FlexItemExpand>` - Same as 'FlexItem' but is hidden by default until expanded (done so by clicking on any FlexRow item)


# Example
```
<FlexTable>
  <FlexHeader>
    <FlexItem>
      ID
    </FlexItem>
    <FlexItem>
      Company
    </FlexItem>
  </FlexHeader>

  <FlexRow>
    <FlexItem>
      fd3gt-1der
    </FlexItem>
    <FlexItem>
      Nixtus
    </FlexItem>
    <FlexItemExpand>
      <!-- THIS WILL BE HIDDEN BY DEFAULT, THEN EXPANDED VISIBLE WHEN FlexRow IS CLICKED -->
      <h1>Company Details</h1>
    </FlexItemExpand>
  </FlexRow>

  <FlexFooter>
    <FlexItem>
      $copy; Nixtus
    </FlexItem>
  </FlexFooter>
</FlexTable>

```


# License

MIT © Andrew Ninneman
MIT © Nixtus LLC

