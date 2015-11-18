# envisa-checkbox-menu

An element for providing access to a persistent model.


## Dependencies

Element dependencies are managed via [Bower](http://bower.io/). You can
install that via:

    npm install -g bower

Then, go ahead and download the element's dependencies:

    bower install


## Playing With Your Element

If you wish to work on your element in isolation, we recommend that you use
[Polyserve](https://github.com/PolymerLabs/polyserve) to keep your element's
bower dependencies in line. You can install it via:

    npm install -g polyserve

And you can run it via:

    polyserve
    
    polyserve -p 9092

Once running, you can preview the element at
`http://localhost:9092/components/envisa-checkbox-menu/demo/`


## Testing Your Element

Simply navigate to the `/test` directory of the element to run its tests. If
you are using Polyserve: `http://localhost:9090/components/envisa-checkbox-menu/test/`

### web-component-tester

The tests are compatible with [web-component-tester](https://github.com/Polymer/web-component-tester).
Install it via:

    npm install -g web-component-tester

Then, you can run your tests on _all_ of your local browsers via:

    wct

#### WCT Tips

`wct -l chrome` will only run tests in chrome.

`wct -p` will keep the browsers alive after test runs (refresh to re-run).

`wct test/some-file.html` will test only the files you specify.


##Deploying Your Element GitHub Page

Move to your development directory:
    
    cd ..
    
If the Polymer Tools hasn't been installed then:

    git clone git://github.com/Polymer/tools.git


Create and enter a temporary directory:

    mkdir temp && cd temp
    
Create SSH Keys via:

    eval `ssh-agent -s` 
    ssh-add ~/.ssh/*_rsa

Publish the GitHub Page (Note: Doing the will both wipe out the temp directory as well as force update the gh-pages branch)

    ../tools/bin/gp.sh <username> <elementname>
    
Remove the temporary directory
   
    cd ..
    rm -rf temp
    
The page will be available at `http://<username>.github.io/<elementname>/`
