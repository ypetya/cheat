--- 
gem: |-
  Install a gem
  
    gem install [gem name]
  
  Update to latest Rubygems (if any):
  
    gem update --system
  
  Search for a gem:
  
    gem query --remote --name [regular expession]
  
  Get list of outdated gems and update as necessary:
  
    gem outdated
  
  Clean up outdated gems:
  
    gem clean
  
  List installed gems by last access time:
  
    gem stale
  
  Current Local Gem Repository:
  
    gem environment
  
    or
  
    ruby -rrubygems -e"puts Gem.path"
  
  Discover Dependency for a Gem:
  
    gem dependency [gem name]
  
  Don't generate Ri and RDoc when installing gems:
  
    gem install [gem name] --no-ri --no-rdoc
  
    to set this as default behavior:
  
    echo "gem: --no-ri --no-rdoc" >> ~/.gemrc
  
  Uninstalling:
  
    gem uninstall [gem name]
  
    if that fails with something like:
    ERROR:  While executing gem ... (Gem::InstallError)
        Unknown gem [gem name]
    then do this...
  
    gem list -d [gem name]
    gem list --local or -l
    gem list --remote or -r
    gem uninstall --install-dir [install directory] [gem name]
  
  Add a repository for remote gems:
  
    gem sources -a [repository url]
