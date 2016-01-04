# Shirt Size CSS
A uniform approach to padding and margin

Who hasn't eyeballed a margin or padding before much to the frustration of the designers? Follow the Shirt Size CSS approach and forget about eyeballing. All you need to do is remember a very simple pattern and get agreement with design on what the base sizes shall be.

[size]-[side*]-[spacing]

**Sizes:** no, xs, small, medium, large, xl, xxl  
**Sides:** top, right, bottom, left, vertical, horizontal (* optional)  
**Spacing:** margin, padding  

Originally created by [Joe Golike](https://github.com/golike)


```less
@baseShirtSize: 16px;

@xs: @baseShirtSize * .25;
@small: @baseShirtSize * .5;
@medium: @baseShirtSize;
@large: @baseShirtSize * 1.5;
@xl: @baseShirtSize * 2;
@xxl: @baseShirtSize * 3;

.auto-margin { margin: auto; }
.auto-top-margin { margin-top: auto; }
.auto-right-margin { margin-right: auto; }
.auto-bottom-margin { margin-bottom: auto; }
.auto-left-margin { margin-left: auto; }
.auto-horizontal-margin { margin-right: auto; margin-left: auto; }
.auto-vertical-margin { margin-top: auto; margin-bottom: auto; }

.no-margin { margin: 0 !important; }
.no-top-margin { margin-top: 0; }
.no-right-margin { margin-right: 0; }
.no-bottom-margin { margin-bottom: 0; }
.no-left-margin { margin-left: 0; }
.no-vertical-margin { margin-top: 0; margin-bottom: 0; }
.no-horizontal-margin { margin-right: 0; margin-left: 0; }

.xs-margin { margin: @xs; }
.xs-top-margin { margin-top: @xs; }
.xs-right-margin { margin-right: @xs; }
.xs-bottom-margin { margin-bottom: @xs; }
.xs-left-margin { margin-left: @xs; }
.xs-vertical-margin { margin-top: @xs; margin-bottom: @xs; }
.xs-horizontal-margin { margin-right: @xs; margin-left: @xs; }

.small-margin { margin: @small; }
.small-top-margin { margin-top: @small; }
.small-right-margin { margin-right: @small; }
.small-bottom-margin { margin-bottom: @small; }
.small-left-margin { margin-left: @small; }
.small-vertical-margin { margin-top: @small; margin-bottom: @small; }
.small-horizontal-margin { margin-right: @small; margin-left: @small; }

.medium-margin { margin: @medium; }
.medium-top-margin { margin-top: @medium; }
.medium-right-margin { margin-right: @medium; }
.medium-bottom-margin { margin-bottom: @medium; }
.medium-left-margin { margin-left: @medium; }
.medium-vertical-margin { margin-top: @medium; margin-bottom: @medium; }
.medium-horizontal-margin { margin-right: @medium; margin-left: @medium; }

.large-margin { margin: @large; }
.large-top-margin { margin-top: @large; }
.large-right-margin { margin-right: @large; }
.large-bottom-margin { margin-bottom: @large; }
.large-left-margin { margin-left: @large; }
.large-vertical-margin { margin-top: @large; margin-bottom: @large; }
.large-horizontal-margin { margin-right: @large; margin-left: @large; }

.xl-margin { margin: @xl; }
.xl-top-margin { margin-top: @xl; }
.xl-right-margin { margin-right: @xl; }
.xl-bottom-margin { margin-bottom: @xl; }
.xl-left-margin { margin-left: @xl; }
.xl-vertical-margin { margin-top: @xl; margin-bottom: @xl; }
.xl-horizontal-margin { margin-right: @xl; margin-left: @xl; }

.xxl-margin { margin: @xxl; }
.xxl-top-margin { margin-top: @xxl; }
.xxl-right-margin { margin-right: @xxl; }
.xxl-bottom-margin { margin-bottom: @xxl; }
.xxl-left-margin { margin-left: @xxl; }
.xxl-vertical-margin { margin-top: @xxl; margin-bottom: @xxl; }
.xxl-horizontal-margin { margin-right: @xxl; margin-left: @xxl; }

.no-padding { padding: 0 !important; }
.no-top-padding { padding-top: 0; }
.no-right-padding { padding-right: 0; }
.no-bottom-padding { padding-bottom: 0; }
.no-left-padding { padding-left: 0; }
.no-vertical-padding { padding-top: 0; padding-bottom: 0; }
.no-horizontal-padding { padding-right: 0; padding-left: 0; }

.xs-padding { padding: @xs; }
.xs-top-padding { padding-top: @xs; }
.xs-right-padding { padding-right: @xs; }
.xs-bottom-padding { padding-bottom: @xs; }
.xs-left-padding { padding-left: @xs; }
.xs-vertical-padding { padding-top: @xs; padding-bottom: @xs; }
.xs-horizontal-padding { padding-right: @xs; padding-left: @xs; }

.small-padding { padding: @small; }
.small-top-padding { padding-top: @small; }
.small-right-padding { padding-right: @small; }
.small-bottom-padding { padding-bottom: @small; }
.small-left-padding { padding-left: @small; }
.small-vertical-padding { padding-top: @small; padding-bottom: @small; }
.small-horizontal-padding { padding-right: @small; padding-left: @small; }

.medium-padding { padding: @medium; }
.medium-top-padding { padding-top: @medium; }
.medium-right-padding { padding-right: @medium; }
.medium-bottom-padding { padding-bottom: @medium; }
.medium-left-padding { padding-left: @medium; }
.medium-vertical-padding { padding-top: @medium; padding-bottom: @medium; }
.medium-horizontal-padding { padding-right: @medium; padding-left: @medium; }

.large-padding { padding: @large; }
.large-top-padding { padding-top: @large; }
.large-right-padding { padding-right: @large; }
.large-bottom-padding { padding-bottom: @large; }
.large-left-padding { padding-left: @large; }
.large-vertical-padding { padding-top: @large; padding-bottom: @large; }
.large-horizontal-padding { padding-right: @large; padding-left: @large; }

.xl-padding { padding: @xl; }
.xl-top-padding { padding-top: @xl; }
.xl-right-padding { padding-right: @xl; }
.xl-bottom-padding { padding-bottom: @xl; }
.xl-left-padding { padding-left: @xl; }
.xl-vertical-padding { padding-top: @xl; padding-bottom: @xl; }
.xl-horizontal-padding { padding-right: @xl; padding-left: @xl; }

.xxl-padding { padding: @xxl; }
.xxl-top-padding { padding-top: @xxl; }
.xxl-right-padding { padding-right: @xxl; }
.xxl-bottom-padding { padding-bottom: @xxl; }
.xxl-left-padding { padding-left: @xxl; }
.xxl-vertical-padding { padding-top: @xxl; padding-bottom: @xxl; }
.xxl-horizontal-padding { padding-right: @xxl; padding-left: @xxl; }
```
