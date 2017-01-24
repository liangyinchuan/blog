# Deployer 4.1.0 release

New version of Deployer 4.1.0 contains a lot of improvements. 

Added support for multiplexing for `NativeSsh`. This feature speeds up deployment process more than 3x times for native ssh type. 

<svg width="607" height="185" viewBox="0 0 607 185" xmlns="http://www.w3.org/2000/svg">
 <g>
  <title>Deployment speed up graph</title>
  <rect stroke="#000" id="svg_1" height="26" width="422.000015" y="23" x="37.5" stroke-width="0" fill="#529D94"/>
  <rect stroke="#000" id="svg_2" height="26" width="119.999988" y="91" x="39.5" stroke-width="0" fill="#EDB6DC"/>
  <path id="svg_3" d="m13.5,311" opacity="0.5" stroke-opacity="null" stroke-width="0" stroke="#000" fill="#619E73"/>
  <line stroke-linecap="null" stroke-linejoin="null" id="svg_5" y2="153" x2="584.508108" y1="153" x1="29.5" fill-opacity="null" stroke-opacity="null" stroke="#000" fill="none"/>
  <text xml:space="preserve" text-anchor="start" font-family="Helvetica, Arial, sans-serif" font-size="12" id="svg_7" y="65.5" x="42" stroke-opacity="null" stroke-width="0" stroke="#000" fill="#444444">Native SSH</text>
  <text xml:space="preserve" text-anchor="start" font-family="Helvetica, Arial, sans-serif" font-size="12" id="svg_8" y="133.5" x="41" stroke-opacity="null" stroke-width="0" stroke="#000" fill="#444444">With SSH multiplexing</text>
  <text xml:space="preserve" text-anchor="start" font-family="Helvetica, Arial, sans-serif" font-size="12" id="svg_9" y="170.5" x="278" stroke-opacity="null" stroke-width="0" stroke="#000" fill="#444444">Deployment time</text>
  <path stroke="#000" transform="rotate(90 590.6399536132814,153.89062500000006) " id="svg_10" d="m585.139966,163.890618l5.5,-19.999992l5.5,19.999992l-11,0z" stroke-opacity="null" stroke-width="0" fill="#444444"/>
 </g>
</svg>

To activate SSH multiplexing, add this line to your `deploy.php` file:

```php
set('ssh_multiplexing', true);
```

Also change log moved from GitHub releases pages to [CHANGELOG.md](https://github.com/deployphp/deployer/blob/master/CHANGELOG.md#v410) file.

To upgrade Deployer run next command:

```sh
dep self-update
```
