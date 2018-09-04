## Contribly AMP example

An AMP validated example of the Contribly contribute widget operating inside an AMP iframe.

[View the working example here.](http://contribly-amp-example.s3-website-eu-west-1.amazonaws.com/)

See the comments in [index.html](index.html) for an explanation of the design considerations.

The AMP iframe is using the Contribly contribute widget iframe wrapper to load the JavaScript contribute widget.
The wrapper registers a Contribly callback to receive notification when the form has been loaded and rendered.
It then measures the height of the form before requesting an AMP iframe resize.

View the source of the [iframe wrapper](https://s3-eu-west-1.amazonaws.com/contribly-widgets/contribute/amp-iframe.html) to see how this is achieved.

AMP may not necessary grant the resize request immediately and is likely to use an AMP iframe overflow to prompt the user to allow the resize.
Additionally AMP may not permit an iframe to reduce in size below it's initial size.

