# Template for generating a simplified printable running order for festivals

## Usage
0. Fork or template this repository. Make sure to include _all_ branches (master and gh-pages).
0. Grant "read and write permissions" to Github Actions (in your fork's "Settings", "Actions", "General").
   This is required to allow the generator workflow to push the generated webpage to Github Pages.
0. Modify running-order.csv with your running order (one act per line; available stages are automatically gathered from the CSV in the order they appear in it).
0. Push your changes. The Github Actions workflow will automatically render them into HTML and publish the result.

## Implementation
This repository contains a Github Actions workflow that pulls https://github.com/n-st/running-order-layout-plain and uses it to render `running-order.csv` into a static HTML page, which is then published via Github Pages.
