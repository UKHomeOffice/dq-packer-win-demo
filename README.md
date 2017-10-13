# dq packer demo

Simple proof of concept packer image that uses a `ubuntu` base image to host a `nginx` webservice with some `ansible` magic.

This demo runs in AWS in the HODAC-DACC-DQ where it makes an ami, though can be forked and run with different aws credentials if desired.

Requires the `AWS_ACCESS_KEY_ID` and `AWS_SECRET_ACCESS_KEY` env vars to be set (or provided via drone secrets)

Build is automated with drone, and only builds on commits/merges to master but will always validate and inspect with output visible in drone.
