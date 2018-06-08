### Manual Installation (all OSes)

1. Install [Node.js](https://nodejs.org/en/). Use the __stable__ version

2. Install [Ruby](https://www.ruby-lang.org/en/documentation/installation/) if it's not already installed on your computer. 

3. Clone this repo and `cd` into the new repo directory:

    ```bash
    git clone git@github.com:GCDigitalFellows/gcdigitalfellows.github.io.git
    cd gcdigitalfellows.github.io
    ```

4. Install node and ruby components inside the repository so that it's specific to the website:

    ```bash
    npm install jekyll
    sudo gem install sass -v 3.4.22
    ```
    
5. Run the update data script 
   ```bash
   node get_data
   ```
 Try to resolve `Error: Cannot find module 'X'` error with `npm install X`. Repeat until all packages are installed. These are some of the packages you may have to install:
 ```bash
 npm install request
 npm install babyparse
 npm install js-yaml
 npm install fs-extra
 npm install escape-html
 ```
 
 Then try to run the site by typing:
 ```bash
 bundle exec jekyll serve
 ```
And then open http://127.0.0.1:4000/ in your web browser.
