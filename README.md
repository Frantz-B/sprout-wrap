# sprout-wrap

[![Build Status](https://travis-ci.org/pivotal-sprout/sprout-wrap.png?branch=master)](https://travis-ci.org/pivotal-sprout/sprout-wrap)

* Bug	KME-5128: Design Issue: table border is not displaying properly in the error banner. (PR - [#6042](https://github.com/KargoGlobal/ControlPanel/pull/6042))






### STORIES
* [KME-4971](https://kargo1.atlassian.net/browse/KME-4971)<a href="http://stackoverflow.com" target="_blank">Go</a>: Deal Group: Add Client Partnerships as new field and relationship (PR - [#5986](https://github.com/KargoGlobal/ControlPanel/pull/5986))
* KME-4970: Campaign: Add Client Partnerships as new field and relationship (PR - [#5981](https://github.com/KargoGlobal/ControlPanel/pull/5981), [#6026](https://github.com/KargoGlobal/ControlPanel/pull/6026))
* KME-4969: Deal Group: Remove Platform Managers and absorb as Client Service Managers in KM (PR - [#5965](https://github.com/KargoGlobal/ControlPanel/pull/5965))
* KME-4921: Repush Failed Error Messaging: Frontend (PR - [#6029](https://github.com/KargoGlobal/ControlPanel/pull/6029), [#5997](https://github.com/KargoGlobal/ControlPanel/pull/5997))
* KME-4919: Creating APIs - IN Hub (PR - [#658](https://github.com/KargoGlobal/integrations-hub/pull/658))


### BUGS
* KME-5128: Design Issue: table border is not displaying properly in the error banner. (PR - [#6042](https://github.com/KargoGlobal/ControlPanel/pull/6042))
* KME-5117: In re-push: Number of the successfully pushed line items banner is not displaying when the failed push banner is displaying. (PR - [#6043](https://github.com/KargoGlobal/ControlPanel/pull/6043))
* KME-5115: On campaign level, placement’s name displays next to each non-pushed LI even when there are multiple non-pushed LIs for the same placement. (PR - [#6039](https://github.com/KargoGlobal/ControlPanel/pull/6039))
* KME-5108: Line items IDs are missing from Error banner. (PR - [#6032](https://github.com/KargoGlobal/ControlPanel/pull/6032))
* KME-5107: Wrong spelling for "Greater" for non-pushed LIs with 0 impressions (PR - [#6032](https://github.com/KargoGlobal/ControlPanel/pull/6032))
* KME-5104: Status Filter in KM not working (PR - [#6036](https://github.com/KargoGlobal/ControlPanel/pull/6036))
* KME-5103: Deal Group: The selected value in 'Client Partnerships' optional field isn't being saved. (PR - [#6033](https://github.com/KargoGlobal/ControlPanel/pull/6033))
* KME-5087: Deal Group: Wrong field for "Client Partnerships" header (PR - [#6033](https://github.com/KargoGlobal/ControlPanel/pull/6033))
* KME-5086: The selected value in 'Client Partnerships' optional field isn't being saved. (PR - [#6033](https://github.com/KargoGlobal/ControlPanel/pull/6033))
* KME-5044: 'Pause' & 'Resume' options are displaying even if the campaign isn't approved. (PR - [#6035](https://github.com/KargoGlobal/ControlPanel/pull/6035))
* KME-4995: Total buffer in media plan tab increases when carving out from a regular line item before saving (PR - [#6031](https://github.com/KargoGlobal/ControlPanel/pull/6031))
* KME-4809: Editing Carve-out line items site list generates new line items (PR - [#6037](https://github.com/KargoGlobal/ControlPanel/pull/6037))
* KME-4789: Tables - Long Line Item Nomenclature Fixing (PR - N/A)
* KME-4532: Manage > Site Lists > Site list builder : (Ad Units) & (Publishers) filters will be reset upon using (Approved for) filter. (PR - [#6022](https://github.com/KargoGlobal/ControlPanel/pull/6022))
* KME-4490: Manage > Campaigns > Specific Campaign > Specific Placement: Trigger toast confirmation for a status failure is displaying in green color. (PR - N/A)










This project uses [soloist](https://github.com/mkocher/soloist) and [librarian-chef](https://github.com/applicationsonline/librarian-chef)
to run a subset of the recipes in sprout's cookbooks.

[Fork it](https://github.com/pivotal-sprout/sprout-wrap/fork) to 
customize its [attributes](http://docs.opscode.com/chef_overview_attributes.html) in [soloistrc](/soloistrc) and the list of recipes 
you'd like to use for your team. You may also want to add other cookbooks to its [Cheffile](/Cheffile), perhaps one 
of the many [community cookbooks](http://community.opscode.com/cookbooks). By default it configures an OS X 
Mavericks workstation for Ruby development.

Finally, if you've never used Chef before - we highly recommend you buy &amp; watch [this excellent 17 minute screencast](http://railscasts.com/episodes/339-chef-solo-basics) by Ryan Bates. 

## Installation under Mavericks (OS X 10.9)

### 1. Install Command Line Tools
  
    xcode-select --install

If you receive a message about the update server being unavailable and are on Mavericks, then you already have the command line tools.

### 2. Clone this project

    git clone https://github.com/pivotal-sprout/sprout-wrap.git
    cd sprout-wrap

### 3. Install soloist & and other required gems

If you're running under rvm or rbenv, you shouldn't preface the following commands with `sudo`.

    sudo gem install bundler
    sudo bundle

If you receive errors like this:

    clang: error: unknown argument: '-multiply_definedsuppress'

then try downgrading those errors like this:

    sudo ARCHFLAGS=-Wno-error=unused-command-line-argument-hard-error-in-future bundle

### 4. Run soloist

[You may want to modify your Energy Saver preferences (**System Preferences &rarr; Energy Saver &rarr; Computer Sleep &rarr; 3hrs**); depending on your network connection, soloist can take from 10 minutes to 2 hours to complete.]

    bundle exec soloist

## Roadmap

See Pivotal Tracker: https://www.pivotaltracker.com/s/projects/884116

## Discussion List

  Join [sprout-users@googlegroups.com](https://groups.google.com/forum/#!forum/sprout-users) if you use Sprout.

## References

* Slides from @hiremaga's [lightning talk on Sprout](http://sprout-talk.cfapps.io/) at Pivotal Labs in June 2013
* [Railscast on chef-solo](http://railscasts.com/episodes/339-chef-solo-basics) by Ryan Bates (PAID)
