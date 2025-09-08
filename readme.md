# Examples of Annotations in Argo apps for Octopus Image Updating.

Examples of annotations used for different image replacement scenarios.

Ultimately we are suggesting leverage aliases to be able to specify the path to a particular file we are providing replacement paths for.

This syntax is similar to how we currently apply image replacement path annotations for `Ref` sources

### Outstanding Questions

- How do we best handle the overlap of implicit ref vs explicit file aliases in annotations.

## Scenarios

 - [Helm Inline Values File]("./helm-inline-values-file/app.yaml) - A Helm source that has a single inline Values file specified.
 - [Helm Inline Values Files](./helm-inline-values-files/app.yaml) - A Helm source with multiple inline values files specified.
 - [Helm Mixed Source Values Files](./helm-mixed-source-values-files/app.yaml) - A Helm sources with a mix of inline and ref based Values files. Also with an [Alternate approach](./helm-mixed-source-values-files/app-alternate.yaml)
 - [Single Ref Path Separated Values Files](./single-ref-path-separated-values/app.yaml) - A single ref is provided that contains multiple values files along different paths.
