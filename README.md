# Configure_ReactJS_Poject
Configurações e preferências de padrões de código em um projeto ReactJS CLI
================================================================================================================================================
1 - Init a project React JS CLI:
	
	- run yarn create react-app name
	
2 - Start project

	- run yarn start

3 - ESLINT:
	
	- install ESLINT:

		- run yarn add eslint -D

		- run yarn eslint --init

		- select: To check syntax, find problems, and enforce code style

		- select: JavaScript modules (import/export)

		- select: React

		- select: Browser

		- select: Use a popular style guides

		- select: Airbnb

		- select: JavaScript
		
4 - Prettier:

	- install Prettier:
	
		- run yarn add prettier eslint-config-prettier eslint-plugin-prettier babel-eslint -D
		
5 - Config .eslintrc.js file:

	module.exports = {
  		env: {
    			browser: true,
    			es2020: true,
  		},
  	extends: [
    		'plugin:react/recommended',
    		'airbnb',
  	],
  	parserOptions: {
    		ecmaFeatures: {
      			jsx: true,
    		},
    		ecmaVersion: 11,
    		sourceType: 'module',
  	},
  	plugins: [
    		'react',
  	],
  	rules: {
  	},
};
