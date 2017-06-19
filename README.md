[![Published on webcomponents.org](https://img.shields.io/badge/webcomponents.org-published-blue.svg)](https://www.webcomponents.org/element/jorgecasar/network-information)

# \<network-information\>

Implements Network Information API, which enables web applications to access information about the network connection in use by the device.

## Installation

First, make sure you have the [Polymer CLI](https://www.npmjs.com/package/polymer-cli) installed. Then run `polymer serve` to serve your element locally.

## Viewing Your Element

```
$ polymer serve
```

## Running Tests

```
$ polymer test
```

Your application is already set up to be tested via [web-component-tester](https://github.com/Polymer/web-component-tester). Run `polymer test` to run your application's test suite locally.

## Usage

<!--
```
<custom-element-demo>
  <template>
    <link rel="import" href="network-information.html">
    <link rel="import" href="../polymer/lib/elements/dom-bind.html">
    <next-code-block></next-code-block>
  </template>
</custom-element-demo>
```
-->
```html
<dom-bind>
  <template>
    <network-information
      api-supported="{{apiSupported}}"
      on-line="{{onLine}}"
      type="{{type}}"
      effective-type="{{effectiveType}}"
      downlink-max="{{downlinkMax}}"
      downlink="{{downlink}}"
      rtt="{{rtt}}">
    </network-information>
    <ul>
      <li>API supported: [[apiSupported]]</li>
      <li>OnLine: [[onLine]]</li>
      <li>Type: [[type]]</li>
      <li>Efective type: [[effectiveType]]</li>
      <li>Downlink Max: [[downlinkMax]]</li>
      <li>Downlink: [[downlink]]</li>
      <li>Rtt: [[rtt]]</li>
    </ul>
  </template>
</dom-bind>
```

## Contributing

1. Fork it!
2. Create your feature branch: `git checkout -b my-new-feature`
3. Commit your changes: `git commit -am 'Add some feature'`
4. Push to the branch: `git push origin my-new-feature`
5. Submit a pull request :D

## Credits

Spec. [Network Information API](https://wicg.github.io/netinfo/).

## License

MIT is open-sourced software licensed under the [MIT license](https://opensource.org/licenses/MIT).
