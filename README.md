# jupyterlab theme base16dark

It uses the jupyterlab dark theme for the main application components, but styles the notebook using Base 16 Tomorrow Night. 

## Installation  

To install the theme and use it right away:  
`jupyter labextension install @ejolly/base16dark`

## Modifying  

Edit any files in the `style` directory (but most likely `variables.css`). Then run the following commands to build the package and enable it for use with jupyterlab:  
1. `npm install` (only need to do once after cloning this repo, not on every change of files)
2. `npm run build`
3. `npm run build:webpack`
4. `jupyter labextension install --debug .` (from within the root directory of this repo)
5. `jupyter lab build` (if you have a jupyterlab instance running already you'll automatically get a notification asking to rebuild, otherwise run this command)

You should now see a new theme option under Settings > JupyterLab Theme. 

## Help

Since jupyterlab is based on React and Material Design we can use the relevant documentation to look up the value of different framework variables:  
- [Colors](https://react-md.mlaursen.com/customization/colors)
