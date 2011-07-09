# Boost Releases

This directory contains Boost Gitian build results, signed by multiple people.

The layout of this directory is:

    <release-name>/
      <signer>/
        boost-build.assert - the result file produced by the signer's build process
        boost-build.assert.sig - the signer's signature certifying the result

This directory is created by the Gitian `gsign` command, after a successful `gbuild`.  It can be verified with `gverify`.

The source is boost-1_43_0.tar.bz2 as obtained from sourceforge.

Normally, all output manifests in the result files should be identical between different signers.

See also:

* [Gitian builder](https://github.com/devrandom/gitian-builder)
