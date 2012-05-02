# A simple application for Medical Diagnostic Devices

This is a simplified model for an application intended to manage the configuration of medical devices for an organization working in the Clinical [In-vitro Diagnotic](http://en.wikipedia.org/wiki/In_vitro_diagnostics) Market. 

The samples are taken from the [company bioMerieux Inc](www.biomerieux.com), based in the RTP Area in NC.


## Resources

The main resource of the application is a medical system. A System is an instrument that the company installs on customer sites (hospital, labs, medical and clinical centers) to perform in-vitro diagnostic tests.  
These systems are built with a number of parts, or components, which are also represented in this model as a resource. Any instrument system may have one or several components attached to them. 
The goal of this application is to allow an instrument administrator in the organization to keep track of all the systems supported by the different business units or areas, and the composition of these systems, that is, all the components defined for each of them. 


You will want to start by [forking](http://help.github.com/fork-a-repo/) this repository so you have your own copy to modify. If you decide to work in a group, I will put a copy of the code in your shared repository. (While it's possible to collaborate with your group by pushing and pulling commits across your two or three separate forks, doing so requires somewhat advanced knowledge of Git and thus isn't expected for this assignment.)

If you're working alone, please **rename your GitHub repository** to something more suitable for your service. You can do this by clicking on the ![admin](/sils-webinfo/election/raw/master/doc/img/admin.png) button from your repository's page on GitHub. A one-word, no-spaces name is best. (If you're working in a group the repository will be named after your group).

## Cloning your project in Cloud9

If you're working alone, and you've successfully forked the repository to your own GitHub account, then cloning your project into Cloud9 is simple. Just sign in to [Cloud9](http://c9.io) using your GitHub account (click the little green [Octocat](http://octodex.github.com/) icon). Your dashboard should open, and you will see a list of `PROJECTS ON GITHUB` on the left. Select your project and click the green `CLONE TO EDIT` button.

If you're in a group, your GitHub repository won't show up in the list of GitHub projects, so you need to click the plus-sign button next to `MY PROJECTS` on the left, and select `Clone From URL`. Then (in another browser tab) go to the homepage of your team's repository, and copy the URL next to where it says `Read+Write access` (it should look something like `git@github.com:sils-webinfo/SteampunkUnicorn.git` if `SteampunkUnicorn` were the name of your group). Go back to Cloud9, paste this URL in the `Source URL` field, and click the green `CHECKOUT` button. Cloud9 should start cloning your project. (Sometimes it flakes out; if it does just try again.)

