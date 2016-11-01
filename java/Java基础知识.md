<!DOCTYPE html>
<html lang="en" class=" is-copy-enabled is-u2f-enabled">
  <head prefix="og: http://ogp.me/ns# fb: http://ogp.me/ns/fb# object: http://ogp.me/ns/object# article: http://ogp.me/ns/article# profile: http://ogp.me/ns/profile#">
    <meta charset='utf-8'>
    

    <link crossorigin="anonymous" href="https://assets-cdn.github.com/assets/frameworks-7a356da712cd13c4e4cfbdc04cf886bb391f84a7e92f9f7b3abf2b1034fea6e9.css" integrity="sha256-ejVtpxLNE8Tkz73ATPiGuzkfhKfpL597Or8rEDT+puk=" media="all" rel="stylesheet" />
    <link crossorigin="anonymous" href="https://assets-cdn.github.com/assets/github-3ca4d5a0760c7ca10f98748867f95c64b034bd809a90302ab1caf3adf1b7845c.css" integrity="sha256-PKTVoHYMfKEPmHSIZ/lcZLA0vYCakDAqscrzrfG3hFw=" media="all" rel="stylesheet" />
    
    
    
    

    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta http-equiv="Content-Language" content="en">
    <meta name="viewport" content="width=device-width">
    
    <title>LearningNotes/Java基础知识.md at master · GeniusVJR/LearningNotes</title>
    <link rel="search" type="application/opensearchdescription+xml" href="/opensearch.xml" title="GitHub">
    <link rel="fluid-icon" href="https://github.com/fluidicon.png" title="GitHub">
    <link rel="apple-touch-icon" href="/apple-touch-icon.png">
    <link rel="apple-touch-icon" sizes="57x57" href="/apple-touch-icon-57x57.png">
    <link rel="apple-touch-icon" sizes="60x60" href="/apple-touch-icon-60x60.png">
    <link rel="apple-touch-icon" sizes="72x72" href="/apple-touch-icon-72x72.png">
    <link rel="apple-touch-icon" sizes="76x76" href="/apple-touch-icon-76x76.png">
    <link rel="apple-touch-icon" sizes="114x114" href="/apple-touch-icon-114x114.png">
    <link rel="apple-touch-icon" sizes="120x120" href="/apple-touch-icon-120x120.png">
    <link rel="apple-touch-icon" sizes="144x144" href="/apple-touch-icon-144x144.png">
    <link rel="apple-touch-icon" sizes="152x152" href="/apple-touch-icon-152x152.png">
    <link rel="apple-touch-icon" sizes="180x180" href="/apple-touch-icon-180x180.png">
    <meta property="fb:app_id" content="1401488693436528">

      <meta content="https://avatars2.githubusercontent.com/u/13393725?v=3&amp;s=400" name="twitter:image:src" /><meta content="@github" name="twitter:site" /><meta content="summary" name="twitter:card" /><meta content="GeniusVJR/LearningNotes" name="twitter:title" /><meta content="LearningNotes - Enjoy Learning." name="twitter:description" />
      <meta content="https://avatars2.githubusercontent.com/u/13393725?v=3&amp;s=400" property="og:image" /><meta content="GitHub" property="og:site_name" /><meta content="object" property="og:type" /><meta content="GeniusVJR/LearningNotes" property="og:title" /><meta content="https://github.com/GeniusVJR/LearningNotes" property="og:url" /><meta content="LearningNotes - Enjoy Learning." property="og:description" />
      <meta name="browser-stats-url" content="https://api.github.com/_private/browser/stats">
    <meta name="browser-errors-url" content="https://api.github.com/_private/browser/errors">
    <link rel="assets" href="https://assets-cdn.github.com/">
    <link rel="web-socket" href="wss://live.github.com/_sockets/ODg0ODM5NjplZWJkZWFkMWMyZmUwYTY3ZDIwMGUxODk2MGU0NmNlZjo3YWMxYTU4OTVjMjk5NzMyYmI0MTVjNzZkNThiYzEwYzQwMDFiZGRmMzc3ODIwYmMyMGZjOGE4YzM5MTA2MDJm--07aacac269a6784926e324f47e7d100b8bc22076">
    <meta name="pjax-timeout" content="1000">
    <link rel="sudo-modal" href="/sessions/sudo_modal">
    <meta name="request-id" content="7CCD5A1B:ADCA:6CEA96A:5818757F" data-pjax-transient>

    <meta name="msapplication-TileImage" content="/windows-tile.png">
    <meta name="msapplication-TileColor" content="#ffffff">
    <meta name="selected-link" value="repo_source" data-pjax-transient>

    <meta name="google-site-verification" content="KT5gs8h0wvaagLKAVWq8bbeNwnZZK1r1XQysX3xurLU">
<meta name="google-site-verification" content="ZzhVyEFwb7w3e0-uOTltm8Jsck2F5StVihD0exw2fsA">
    <meta name="google-analytics" content="UA-3769691-2">

<meta content="collector.githubapp.com" name="octolytics-host" /><meta content="github" name="octolytics-app-id" /><meta content="7CCD5A1B:ADCA:6CEA96A:5818757F" name="octolytics-dimension-request_id" /><meta content="8848396" name="octolytics-actor-id" /><meta content="vip365" name="octolytics-actor-login" /><meta content="39eba32b737b0ddd90f1e629f705aeb8eeee98b9b80313e2760fbe4ba3bf0e94" name="octolytics-actor-hash" />
<meta content="/&lt;user-name&gt;/&lt;repo-name&gt;/blob/show" data-pjax-transient="true" name="analytics-location" />



  <meta class="js-ga-set" name="dimension1" content="Logged In">



        <meta name="hostname" content="github.com">
    <meta name="user-login" content="vip365">

        <meta name="expected-hostname" content="github.com">
      <meta name="js-proxy-site-detection-payload" content="OWQyM2EwYmE0ZTIyNTdjNjRmNWJiYTZlNWFhZTU4NmJlZWFkNzA1N2QzYmY2ZTYyYjBlOTI4NWNjMmM2YzE3ZXx7InJlbW90ZV9hZGRyZXNzIjoiMTI0LjIwNS45MC4yNyIsInJlcXVlc3RfaWQiOiI3Q0NENUExQjpBRENBOjZDRUE5NkE6NTgxODc1N0YiLCJ0aW1lc3RhbXAiOjE0Nzc5OTc5NTIsImhvc3QiOiJnaXRodWIuY29tIn0=">


      <link rel="mask-icon" href="https://assets-cdn.github.com/pinned-octocat.svg" color="#4078c0">
      <link rel="icon" type="image/x-icon" href="https://assets-cdn.github.com/favicon.ico">

    <meta name="html-safe-nonce" content="7b2299741aaf8ff1db77b22f18ce6133dd77af35">
    <meta content="ac627e2bd3e01a6c163de6f861a275d912e8c9c6" name="form-nonce" />

    <meta http-equiv="x-pjax-version" content="7169aff4fa8a37321cf85a00a41beb6d">
    

      
  <meta name="description" content="LearningNotes - Enjoy Learning.">
  <meta name="go-import" content="github.com/GeniusVJR/LearningNotes git https://github.com/GeniusVJR/LearningNotes.git">

  <meta content="13393725" name="octolytics-dimension-user_id" /><meta content="GeniusVJR" name="octolytics-dimension-user_login" /><meta content="60711512" name="octolytics-dimension-repository_id" /><meta content="GeniusVJR/LearningNotes" name="octolytics-dimension-repository_nwo" /><meta content="true" name="octolytics-dimension-repository_public" /><meta content="false" name="octolytics-dimension-repository_is_fork" /><meta content="60711512" name="octolytics-dimension-repository_network_root_id" /><meta content="GeniusVJR/LearningNotes" name="octolytics-dimension-repository_network_root_nwo" />
  <link href="https://github.com/GeniusVJR/LearningNotes/commits/master.atom" rel="alternate" title="Recent Commits to LearningNotes:master" type="application/atom+xml">


      <link rel="canonical" href="https://github.com/GeniusVJR/LearningNotes/blob/master/Part2/JavaSE/Java%E5%9F%BA%E7%A1%80%E7%9F%A5%E8%AF%86.md" data-pjax-transient>
  </head>


  <body class="logged-in  env-production windows vis-public page-blob">
    <div id="js-pjax-loader-bar" class="pjax-loader-bar"><div class="progress"></div></div>
    <a href="#start-of-content" tabindex="1" class="accessibility-aid js-skip-to-content">Skip to content</a>

    
    
    



        <div class="header header-logged-in true" role="banner">
  <div class="container clearfix">

    <a class="header-logo-invertocat" href="https://github.com/" data-hotkey="g d" aria-label="Homepage" data-ga-click="Header, go to dashboard, icon:logo">
  <svg aria-hidden="true" class="octicon octicon-mark-github" height="28" version="1.1" viewBox="0 0 16 16" width="28"><path d="M8 0C3.58 0 0 3.58 0 8c0 3.54 2.29 6.53 5.47 7.59.4.07.55-.17.55-.38 0-.19-.01-.82-.01-1.49-2.01.37-2.53-.49-2.69-.94-.09-.23-.48-.94-.82-1.13-.28-.15-.68-.52-.01-.53.63-.01 1.08.58 1.23.82.72 1.21 1.87.87 2.33.66.07-.52.28-.87.51-1.07-1.78-.2-3.64-.89-3.64-3.95 0-.87.31-1.59.82-2.15-.08-.2-.36-1.02.08-2.12 0 0 .67-.21 2.2.82.64-.18 1.32-.27 2-.27.68 0 1.36.09 2 .27 1.53-1.04 2.2-.82 2.2-.82.44 1.1.16 1.92.08 2.12.51.56.82 1.27.82 2.15 0 3.07-1.87 3.75-3.65 3.95.29.25.54.73.54 1.48 0 1.07-.01 1.93-.01 2.2 0 .21.15.46.55.38A8.013 8.013 0 0 0 16 8c0-4.42-3.58-8-8-8z"></path></svg>
</a>


        <div class="header-search scoped-search site-scoped-search js-site-search" role="search">
  <!-- '"` --><!-- </textarea></xmp> --></option></form><form accept-charset="UTF-8" action="/GeniusVJR/LearningNotes/search" class="js-site-search-form" data-scoped-search-url="/GeniusVJR/LearningNotes/search" data-unscoped-search-url="/search" method="get"><div style="margin:0;padding:0;display:inline"><input name="utf8" type="hidden" value="&#x2713;" /></div>
    <label class="form-control header-search-wrapper js-chromeless-input-container">
      <div class="header-search-scope">This repository</div>
      <input type="text"
        class="form-control header-search-input js-site-search-focus js-site-search-field is-clearable"
        data-hotkey="s"
        name="q"
        placeholder="Search"
        aria-label="Search this repository"
        data-unscoped-placeholder="Search GitHub"
        data-scoped-placeholder="Search"
        autocapitalize="off">
    </label>
</form></div>


      <ul class="header-nav float-left" role="navigation">
        <li class="header-nav-item">
          <a href="/pulls" aria-label="Pull requests you created" class="js-selected-navigation-item header-nav-link" data-ga-click="Header, click, Nav menu - item:pulls context:user" data-hotkey="g p" data-selected-links="/pulls /pulls/assigned /pulls/mentioned /pulls">
            Pull requests
</a>        </li>
        <li class="header-nav-item">
          <a href="/issues" aria-label="Issues you created" class="js-selected-navigation-item header-nav-link" data-ga-click="Header, click, Nav menu - item:issues context:user" data-hotkey="g i" data-selected-links="/issues /issues/assigned /issues/mentioned /issues">
            Issues
</a>        </li>
          <li class="header-nav-item">
            <a class="header-nav-link" href="https://gist.github.com/" data-ga-click="Header, go to gist, text:gist">Gist</a>
          </li>
      </ul>

    
<ul class="header-nav user-nav float-right" id="user-links">
  <li class="header-nav-item">
    
    <a href="/notifications" aria-label="You have no unread notifications" class="header-nav-link notification-indicator tooltipped tooltipped-s js-socket-channel js-notification-indicator" data-channel="tenant:1:notification-changed:8848396" data-ga-click="Header, go to notifications, icon:read" data-hotkey="g n">
        <span class="mail-status "></span>
        <svg aria-hidden="true" class="octicon octicon-bell" height="16" version="1.1" viewBox="0 0 14 16" width="14"><path d="M14 12v1H0v-1l.73-.58c.77-.77.81-2.55 1.19-4.42C2.69 3.23 6 2 6 2c0-.55.45-1 1-1s1 .45 1 1c0 0 3.39 1.23 4.16 5 .38 1.88.42 3.66 1.19 4.42l.66.58H14zm-7 4c1.11 0 2-.89 2-2H5c0 1.11.89 2 2 2z"></path></svg>
</a>
  </li>

  <li class="header-nav-item dropdown js-menu-container">
    <a class="header-nav-link tooltipped tooltipped-s js-menu-target" href="/new"
       aria-label="Create new…"
       data-ga-click="Header, create new, icon:add">
      <svg aria-hidden="true" class="octicon octicon-plus float-left" height="16" version="1.1" viewBox="0 0 12 16" width="12"><path d="M12 9H7v5H5V9H0V7h5V2h2v5h5z"></path></svg>
      <span class="dropdown-caret"></span>
    </a>

    <div class="dropdown-menu-content js-menu-content">
      <ul class="dropdown-menu dropdown-menu-sw">
        
<a class="dropdown-item" href="/new" data-ga-click="Header, create new repository">
  New repository
</a>

  <a class="dropdown-item" href="/new/import" data-ga-click="Header, import a repository">
    Import repository
  </a>


  <a class="dropdown-item" href="/organizations/new" data-ga-click="Header, create new organization">
    New organization
  </a>



  <div class="dropdown-divider"></div>
  <div class="dropdown-header">
    <span title="GeniusVJR/LearningNotes">This repository</span>
  </div>
    <a class="dropdown-item" href="/GeniusVJR/LearningNotes/issues/new" data-ga-click="Header, create new issue">
      New issue
    </a>

      </ul>
    </div>
  </li>

  <li class="header-nav-item dropdown js-menu-container">
    <a class="header-nav-link name tooltipped tooltipped-sw js-menu-target" href="/vip365"
       aria-label="View profile and more"
       data-ga-click="Header, show menu, icon:avatar">
      <img alt="@vip365" class="avatar" height="20" src="https://avatars3.githubusercontent.com/u/8848396?v=3&amp;s=40" width="20" />
      <span class="dropdown-caret"></span>
    </a>

    <div class="dropdown-menu-content js-menu-content">
      <div class="dropdown-menu dropdown-menu-sw">
        <div class="dropdown-header header-nav-current-user css-truncate">
          Signed in as <strong class="css-truncate-target">vip365</strong>
        </div>

        <div class="dropdown-divider"></div>

        <a class="dropdown-item" href="/vip365" data-ga-click="Header, go to profile, text:your profile">
          Your profile
        </a>
        <a class="dropdown-item" href="/vip365?tab=stars" data-ga-click="Header, go to starred repos, text:your stars">
          Your stars
        </a>
        <a class="dropdown-item" href="/explore" data-ga-click="Header, go to explore, text:explore">
          Explore
        </a>
          <a class="dropdown-item" href="/integrations" data-ga-click="Header, go to integrations, text:integrations">
            Integrations
          </a>
        <a class="dropdown-item" href="https://help.github.com" data-ga-click="Header, go to help, text:help">
          Help
        </a>

        <div class="dropdown-divider"></div>

        <a class="dropdown-item" href="/settings/profile" data-ga-click="Header, go to settings, icon:settings">
          Settings
        </a>

        <!-- '"` --><!-- </textarea></xmp> --></option></form><form accept-charset="UTF-8" action="/logout" class="logout-form" data-form-nonce="ac627e2bd3e01a6c163de6f861a275d912e8c9c6" method="post"><div style="margin:0;padding:0;display:inline"><input name="utf8" type="hidden" value="&#x2713;" /><input name="authenticity_token" type="hidden" value="gWsZwBWIXMaW0aQWUx5kZOabV5cTPkxqBzS14zjoAteCOy/0sZ+7VjgsnLvVCgQbvYW5G3DpsI2wClFccGzRNw==" /></div>
          <button type="submit" class="dropdown-item dropdown-signout" data-ga-click="Header, sign out, icon:logout">
            Sign out
          </button>
</form>      </div>
    </div>
  </li>
</ul>


    
  </div>
</div>


      


    <div id="start-of-content" class="accessibility-aid"></div>

      <div id="js-flash-container">
</div>


    <div role="main">
        <div itemscope itemtype="http://schema.org/SoftwareSourceCode">
    <div id="js-repo-pjax-container" data-pjax-container>
      
<div class="pagehead repohead instapaper_ignore readability-menu experiment-repo-nav">
  <div class="container repohead-details-container">

    

<ul class="pagehead-actions">

  <li>
        <!-- '"` --><!-- </textarea></xmp> --></option></form><form accept-charset="UTF-8" action="/notifications/subscribe" class="js-social-container" data-autosubmit="true" data-form-nonce="ac627e2bd3e01a6c163de6f861a275d912e8c9c6" data-remote="true" method="post"><div style="margin:0;padding:0;display:inline"><input name="utf8" type="hidden" value="&#x2713;" /><input name="authenticity_token" type="hidden" value="vWCBzAG/SMvodbVjfB/ESov1jdIL6FPyew9pnKpekk+7fPSt+OYVrYkl0ou7LjqvrJJ7SoXFmxd4ZGXVp0q85w==" /></div>      <input class="form-control" id="repository_id" name="repository_id" type="hidden" value="60711512" />

        <div class="select-menu js-menu-container js-select-menu">
          <a href="/GeniusVJR/LearningNotes/subscription"
            class="btn btn-sm btn-with-count select-menu-button js-menu-target" role="button" tabindex="0" aria-haspopup="true"
            data-ga-click="Repository, click Watch settings, action:blob#show">
            <span class="js-select-button">
              <svg aria-hidden="true" class="octicon octicon-eye" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path d="M8.06 2C3 2 0 8 0 8s3 6 8.06 6C13 14 16 8 16 8s-3-6-7.94-6zM8 12c-2.2 0-4-1.78-4-4 0-2.2 1.8-4 4-4 2.22 0 4 1.8 4 4 0 2.22-1.78 4-4 4zm2-4c0 1.11-.89 2-2 2-1.11 0-2-.89-2-2 0-1.11.89-2 2-2 1.11 0 2 .89 2 2z"></path></svg>
              Watch
            </span>
          </a>
          <a class="social-count js-social-count"
            href="/GeniusVJR/LearningNotes/watchers"
            aria-label="358 users are watching this repository">
            358
          </a>

        <div class="select-menu-modal-holder">
          <div class="select-menu-modal subscription-menu-modal js-menu-content" aria-hidden="true">
            <div class="select-menu-header js-navigation-enable" tabindex="-1">
              <svg aria-label="Close" class="octicon octicon-x js-menu-close" height="16" role="img" version="1.1" viewBox="0 0 12 16" width="12"><path d="M7.48 8l3.75 3.75-1.48 1.48L6 9.48l-3.75 3.75-1.48-1.48L4.52 8 .77 4.25l1.48-1.48L6 6.52l3.75-3.75 1.48 1.48z"></path></svg>
              <span class="select-menu-title">Notifications</span>
            </div>

              <div class="select-menu-list js-navigation-container" role="menu">

                <div class="select-menu-item js-navigation-item selected" role="menuitem" tabindex="0">
                  <svg aria-hidden="true" class="octicon octicon-check select-menu-item-icon" height="16" version="1.1" viewBox="0 0 12 16" width="12"><path d="M12 5l-8 8-4-4 1.5-1.5L4 10l6.5-6.5z"></path></svg>
                  <div class="select-menu-item-text">
                    <input checked="checked" id="do_included" name="do" type="radio" value="included" />
                    <span class="select-menu-item-heading">Not watching</span>
                    <span class="description">Be notified when participating or @mentioned.</span>
                    <span class="js-select-button-text hidden-select-button-text">
                      <svg aria-hidden="true" class="octicon octicon-eye" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path d="M8.06 2C3 2 0 8 0 8s3 6 8.06 6C13 14 16 8 16 8s-3-6-7.94-6zM8 12c-2.2 0-4-1.78-4-4 0-2.2 1.8-4 4-4 2.22 0 4 1.8 4 4 0 2.22-1.78 4-4 4zm2-4c0 1.11-.89 2-2 2-1.11 0-2-.89-2-2 0-1.11.89-2 2-2 1.11 0 2 .89 2 2z"></path></svg>
                      Watch
                    </span>
                  </div>
                </div>

                <div class="select-menu-item js-navigation-item " role="menuitem" tabindex="0">
                  <svg aria-hidden="true" class="octicon octicon-check select-menu-item-icon" height="16" version="1.1" viewBox="0 0 12 16" width="12"><path d="M12 5l-8 8-4-4 1.5-1.5L4 10l6.5-6.5z"></path></svg>
                  <div class="select-menu-item-text">
                    <input id="do_subscribed" name="do" type="radio" value="subscribed" />
                    <span class="select-menu-item-heading">Watching</span>
                    <span class="description">Be notified of all conversations.</span>
                    <span class="js-select-button-text hidden-select-button-text">
                      <svg aria-hidden="true" class="octicon octicon-eye" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path d="M8.06 2C3 2 0 8 0 8s3 6 8.06 6C13 14 16 8 16 8s-3-6-7.94-6zM8 12c-2.2 0-4-1.78-4-4 0-2.2 1.8-4 4-4 2.22 0 4 1.8 4 4 0 2.22-1.78 4-4 4zm2-4c0 1.11-.89 2-2 2-1.11 0-2-.89-2-2 0-1.11.89-2 2-2 1.11 0 2 .89 2 2z"></path></svg>
                      Unwatch
                    </span>
                  </div>
                </div>

                <div class="select-menu-item js-navigation-item " role="menuitem" tabindex="0">
                  <svg aria-hidden="true" class="octicon octicon-check select-menu-item-icon" height="16" version="1.1" viewBox="0 0 12 16" width="12"><path d="M12 5l-8 8-4-4 1.5-1.5L4 10l6.5-6.5z"></path></svg>
                  <div class="select-menu-item-text">
                    <input id="do_ignore" name="do" type="radio" value="ignore" />
                    <span class="select-menu-item-heading">Ignoring</span>
                    <span class="description">Never be notified.</span>
                    <span class="js-select-button-text hidden-select-button-text">
                      <svg aria-hidden="true" class="octicon octicon-mute" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path d="M8 2.81v10.38c0 .67-.81 1-1.28.53L3 10H1c-.55 0-1-.45-1-1V7c0-.55.45-1 1-1h2l3.72-3.72C7.19 1.81 8 2.14 8 2.81zm7.53 3.22l-1.06-1.06-1.97 1.97-1.97-1.97-1.06 1.06L11.44 8 9.47 9.97l1.06 1.06 1.97-1.97 1.97 1.97 1.06-1.06L13.56 8l1.97-1.97z"></path></svg>
                      Stop ignoring
                    </span>
                  </div>
                </div>

              </div>

            </div>
          </div>
        </div>
</form>
  </li>

  <li>
    
  <div class="js-toggler-container js-social-container starring-container ">

    <!-- '"` --><!-- </textarea></xmp> --></option></form><form accept-charset="UTF-8" action="/GeniusVJR/LearningNotes/unstar" class="starred" data-form-nonce="ac627e2bd3e01a6c163de6f861a275d912e8c9c6" data-remote="true" method="post"><div style="margin:0;padding:0;display:inline"><input name="utf8" type="hidden" value="&#x2713;" /><input name="authenticity_token" type="hidden" value="6EuPptjyRcfCkbE8Jy5eNoOkYM29uE+mkaz1xeZKE+SznBbGsU0AHTYpMSGXjxfXTjOFpLun1KvDkGZQ8xFFrQ==" /></div>
      <button
        type="submit"
        class="btn btn-sm btn-with-count js-toggler-target"
        aria-label="Unstar this repository" title="Unstar GeniusVJR/LearningNotes"
        data-ga-click="Repository, click unstar button, action:blob#show; text:Unstar">
        <svg aria-hidden="true" class="octicon octicon-star" height="16" version="1.1" viewBox="0 0 14 16" width="14"><path d="M14 6l-4.9-.64L7 1 4.9 5.36 0 6l3.6 3.26L2.67 14 7 11.67 11.33 14l-.93-4.74z"></path></svg>
        Unstar
      </button>
        <a class="social-count js-social-count" href="/GeniusVJR/LearningNotes/stargazers"
           aria-label="3267 users starred this repository">
          3,267
        </a>
</form>
    <!-- '"` --><!-- </textarea></xmp> --></option></form><form accept-charset="UTF-8" action="/GeniusVJR/LearningNotes/star" class="unstarred" data-form-nonce="ac627e2bd3e01a6c163de6f861a275d912e8c9c6" data-remote="true" method="post"><div style="margin:0;padding:0;display:inline"><input name="utf8" type="hidden" value="&#x2713;" /><input name="authenticity_token" type="hidden" value="IJKwA1Jg8RSBilbu9ywDx7Z6pkogXonAduJ6YWEqiwuH/6zne37nREshIRfzzj1YO1AJMTAC6ZTPzoF4oWtTGg==" /></div>
      <button
        type="submit"
        class="btn btn-sm btn-with-count js-toggler-target"
        aria-label="Star this repository" title="Star GeniusVJR/LearningNotes"
        data-ga-click="Repository, click star button, action:blob#show; text:Star">
        <svg aria-hidden="true" class="octicon octicon-star" height="16" version="1.1" viewBox="0 0 14 16" width="14"><path d="M14 6l-4.9-.64L7 1 4.9 5.36 0 6l3.6 3.26L2.67 14 7 11.67 11.33 14l-.93-4.74z"></path></svg>
        Star
      </button>
        <a class="social-count js-social-count" href="/GeniusVJR/LearningNotes/stargazers"
           aria-label="3267 users starred this repository">
          3,267
        </a>
</form>  </div>

  </li>

  <li>
          <!-- '"` --><!-- </textarea></xmp> --></option></form><form accept-charset="UTF-8" action="/GeniusVJR/LearningNotes/fork" class="btn-with-count" data-form-nonce="ac627e2bd3e01a6c163de6f861a275d912e8c9c6" method="post"><div style="margin:0;padding:0;display:inline"><input name="utf8" type="hidden" value="&#x2713;" /><input name="authenticity_token" type="hidden" value="qk2A16YAoPDSnfsqTu/UFTxA8k/EZgi90hwpcbqt31RH9jPHN/TdfS52OJk/hUuVqFs/ujN0ftqeUi00GLVg+w==" /></div>
            <button
                type="submit"
                class="btn btn-sm btn-with-count"
                data-ga-click="Repository, show fork modal, action:blob#show; text:Fork"
                title="Fork your own copy of GeniusVJR/LearningNotes to your account"
                aria-label="Fork your own copy of GeniusVJR/LearningNotes to your account">
              <svg aria-hidden="true" class="octicon octicon-repo-forked" height="16" version="1.1" viewBox="0 0 10 16" width="10"><path d="M8 1a1.993 1.993 0 0 0-1 3.72V6L5 8 3 6V4.72A1.993 1.993 0 0 0 2 1a1.993 1.993 0 0 0-1 3.72V6.5l3 3v1.78A1.993 1.993 0 0 0 5 15a1.993 1.993 0 0 0 1-3.72V9.5l3-3V4.72A1.993 1.993 0 0 0 8 1zM2 4.2C1.34 4.2.8 3.65.8 3c0-.65.55-1.2 1.2-1.2.65 0 1.2.55 1.2 1.2 0 .65-.55 1.2-1.2 1.2zm3 10c-.66 0-1.2-.55-1.2-1.2 0-.65.55-1.2 1.2-1.2.65 0 1.2.55 1.2 1.2 0 .65-.55 1.2-1.2 1.2zm3-10c-.66 0-1.2-.55-1.2-1.2 0-.65.55-1.2 1.2-1.2.65 0 1.2.55 1.2 1.2 0 .65-.55 1.2-1.2 1.2z"></path></svg>
              Fork
            </button>
</form>
    <a href="/GeniusVJR/LearningNotes/network" class="social-count"
       aria-label="1220 users are forked this repository">
      1,220
    </a>
  </li>
</ul>

    <h1 class="public ">
  <svg aria-hidden="true" class="octicon octicon-repo" height="16" version="1.1" viewBox="0 0 12 16" width="12"><path d="M4 9H3V8h1v1zm0-3H3v1h1V6zm0-2H3v1h1V4zm0-2H3v1h1V2zm8-1v12c0 .55-.45 1-1 1H6v2l-1.5-1.5L3 16v-2H1c-.55 0-1-.45-1-1V1c0-.55.45-1 1-1h10c.55 0 1 .45 1 1zm-1 10H1v2h2v-1h3v1h5v-2zm0-10H2v9h9V1z"></path></svg>
  <span class="author" itemprop="author"><a href="/GeniusVJR" class="url fn" rel="author">GeniusVJR</a></span><!--
--><span class="path-divider">/</span><!--
--><strong itemprop="name"><a href="/GeniusVJR/LearningNotes" data-pjax="#js-repo-pjax-container">LearningNotes</a></strong>

</h1>

  </div>
  <div class="container">
    
<nav class="reponav js-repo-nav js-sidenav-container-pjax"
     itemscope
     itemtype="http://schema.org/BreadcrumbList"
     role="navigation"
     data-pjax="#js-repo-pjax-container">

  <span itemscope itemtype="http://schema.org/ListItem" itemprop="itemListElement">
    <a href="/GeniusVJR/LearningNotes" aria-selected="true" class="js-selected-navigation-item selected reponav-item" data-hotkey="g c" data-selected-links="repo_source repo_downloads repo_commits repo_releases repo_tags repo_branches /GeniusVJR/LearningNotes" itemprop="url">
      <svg aria-hidden="true" class="octicon octicon-code" height="16" version="1.1" viewBox="0 0 14 16" width="14"><path d="M9.5 3L8 4.5 11.5 8 8 11.5 9.5 13 14 8 9.5 3zm-5 0L0 8l4.5 5L6 11.5 2.5 8 6 4.5 4.5 3z"></path></svg>
      <span itemprop="name">Code</span>
      <meta itemprop="position" content="1">
</a>  </span>

    <span itemscope itemtype="http://schema.org/ListItem" itemprop="itemListElement">
      <a href="/GeniusVJR/LearningNotes/issues" class="js-selected-navigation-item reponav-item" data-hotkey="g i" data-selected-links="repo_issues repo_labels repo_milestones /GeniusVJR/LearningNotes/issues" itemprop="url">
        <svg aria-hidden="true" class="octicon octicon-issue-opened" height="16" version="1.1" viewBox="0 0 14 16" width="14"><path d="M7 2.3c3.14 0 5.7 2.56 5.7 5.7s-2.56 5.7-5.7 5.7A5.71 5.71 0 0 1 1.3 8c0-3.14 2.56-5.7 5.7-5.7zM7 1C3.14 1 0 4.14 0 8s3.14 7 7 7 7-3.14 7-7-3.14-7-7-7zm1 3H6v5h2V4zm0 6H6v2h2v-2z"></path></svg>
        <span itemprop="name">Issues</span>
        <span class="counter">15</span>
        <meta itemprop="position" content="2">
</a>    </span>

  <span itemscope itemtype="http://schema.org/ListItem" itemprop="itemListElement">
    <a href="/GeniusVJR/LearningNotes/pulls" class="js-selected-navigation-item reponav-item" data-hotkey="g p" data-selected-links="repo_pulls /GeniusVJR/LearningNotes/pulls" itemprop="url">
      <svg aria-hidden="true" class="octicon octicon-git-pull-request" height="16" version="1.1" viewBox="0 0 12 16" width="12"><path d="M11 11.28V5c-.03-.78-.34-1.47-.94-2.06C9.46 2.35 8.78 2.03 8 2H7V0L4 3l3 3V4h1c.27.02.48.11.69.31.21.2.3.42.31.69v6.28A1.993 1.993 0 0 0 10 15a1.993 1.993 0 0 0 1-3.72zm-1 2.92c-.66 0-1.2-.55-1.2-1.2 0-.65.55-1.2 1.2-1.2.65 0 1.2.55 1.2 1.2 0 .65-.55 1.2-1.2 1.2zM4 3c0-1.11-.89-2-2-2a1.993 1.993 0 0 0-1 3.72v6.56A1.993 1.993 0 0 0 2 15a1.993 1.993 0 0 0 1-3.72V4.72c.59-.34 1-.98 1-1.72zm-.8 10c0 .66-.55 1.2-1.2 1.2-.65 0-1.2-.55-1.2-1.2 0-.65.55-1.2 1.2-1.2.65 0 1.2.55 1.2 1.2zM2 4.2C1.34 4.2.8 3.65.8 3c0-.65.55-1.2 1.2-1.2.65 0 1.2.55 1.2 1.2 0 .65-.55 1.2-1.2 1.2z"></path></svg>
      <span itemprop="name">Pull requests</span>
      <span class="counter">1</span>
      <meta itemprop="position" content="3">
</a>  </span>

  <a href="/GeniusVJR/LearningNotes/projects" class="js-selected-navigation-item reponav-item" data-selected-links="repo_projects new_repo_project repo_project /GeniusVJR/LearningNotes/projects">
    <svg class="octicon" aria-hidden="true" version="1.1" width="15" height="16" viewBox="0 0 15 16">
      <path d="M1 15h13V1H1v14zM15 1v14a1 1 0 0 1-1 1H1a1 1 0 0 1-1-1V1a1 1 0 0 1 1-1h13a1 1 0 0 1 1 1zm-4.41 11h1.82c.59 0 .59-.41.59-1V3c0-.59 0-1-.59-1h-1.82C10 2 10 2.41 10 3v8c0 .59 0 1 .59 1zm-4-2h1.82C9 10 9 9.59 9 9V3c0-.59 0-1-.59-1H6.59C6 2 6 2.41 6 3v6c0 .59 0 1 .59 1zM2 13V3c0-.59 0-1 .59-1h1.82C5 2 5 2.41 5 3v10c0 .59 0 1-.59 1H2.59C2 14 2 13.59 2 13z"></path>
    </svg>
    Projects
    <span class="counter">0</span>
</a>
    <a href="/GeniusVJR/LearningNotes/wiki" class="js-selected-navigation-item reponav-item" data-hotkey="g w" data-selected-links="repo_wiki /GeniusVJR/LearningNotes/wiki">
      <svg aria-hidden="true" class="octicon octicon-book" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path d="M3 5h4v1H3V5zm0 3h4V7H3v1zm0 2h4V9H3v1zm11-5h-4v1h4V5zm0 2h-4v1h4V7zm0 2h-4v1h4V9zm2-6v9c0 .55-.45 1-1 1H9.5l-1 1-1-1H2c-.55 0-1-.45-1-1V3c0-.55.45-1 1-1h5.5l1 1 1-1H15c.55 0 1 .45 1 1zm-8 .5L7.5 3H2v9h6V3.5zm7-.5H9.5l-.5.5V12h6V3z"></path></svg>
      Wiki
</a>

  <a href="/GeniusVJR/LearningNotes/pulse" class="js-selected-navigation-item reponav-item" data-selected-links="pulse /GeniusVJR/LearningNotes/pulse">
    <svg aria-hidden="true" class="octicon octicon-pulse" height="16" version="1.1" viewBox="0 0 14 16" width="14"><path d="M11.5 8L8.8 5.4 6.6 8.5 5.5 1.6 2.38 8H0v2h3.6l.9-1.8.9 5.4L9 8.5l1.6 1.5H14V8z"></path></svg>
    Pulse
</a>
  <a href="/GeniusVJR/LearningNotes/graphs" class="js-selected-navigation-item reponav-item" data-selected-links="repo_graphs repo_contributors /GeniusVJR/LearningNotes/graphs">
    <svg aria-hidden="true" class="octicon octicon-graph" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path d="M16 14v1H0V0h1v14h15zM5 13H3V8h2v5zm4 0H7V3h2v10zm4 0h-2V6h2v7z"></path></svg>
    Graphs
</a>

</nav>

  </div>
</div>

<div class="container new-discussion-timeline experiment-repo-nav">
  <div class="repository-content">

    

<a href="/GeniusVJR/LearningNotes/blob/1170fc20a16edff3f4edd8acb9b500521115a18b/Part2/JavaSE/Java%E5%9F%BA%E7%A1%80%E7%9F%A5%E8%AF%86.md" class="d-none js-permalink-shortcut" data-hotkey="y">Permalink</a>

<!-- blob contrib key: blob_contributors:v21:3c95e3a885a2cd96c7e365857a55c189 -->

<div class="file-navigation js-zeroclipboard-container">
  
<div class="select-menu branch-select-menu js-menu-container js-select-menu float-left">
  <button class="btn btn-sm select-menu-button js-menu-target css-truncate" data-hotkey="w"
    
    type="button" aria-label="Switch branches or tags" tabindex="0" aria-haspopup="true">
    <i>Branch:</i>
    <span class="js-select-button css-truncate-target">master</span>
  </button>

  <div class="select-menu-modal-holder js-menu-content js-navigation-container" data-pjax aria-hidden="true">

    <div class="select-menu-modal">
      <div class="select-menu-header">
        <svg aria-label="Close" class="octicon octicon-x js-menu-close" height="16" role="img" version="1.1" viewBox="0 0 12 16" width="12"><path d="M7.48 8l3.75 3.75-1.48 1.48L6 9.48l-3.75 3.75-1.48-1.48L4.52 8 .77 4.25l1.48-1.48L6 6.52l3.75-3.75 1.48 1.48z"></path></svg>
        <span class="select-menu-title">Switch branches/tags</span>
      </div>

      <div class="select-menu-filters">
        <div class="select-menu-text-filter">
          <input type="text" aria-label="Filter branches/tags" id="context-commitish-filter-field" class="form-control js-filterable-field js-navigation-enable" placeholder="Filter branches/tags">
        </div>
        <div class="select-menu-tabs">
          <ul>
            <li class="select-menu-tab">
              <a href="#" data-tab-filter="branches" data-filter-placeholder="Filter branches/tags" class="js-select-menu-tab" role="tab">Branches</a>
            </li>
            <li class="select-menu-tab">
              <a href="#" data-tab-filter="tags" data-filter-placeholder="Find a tag…" class="js-select-menu-tab" role="tab">Tags</a>
            </li>
          </ul>
        </div>
      </div>

      <div class="select-menu-list select-menu-tab-bucket js-select-menu-tab-bucket" data-tab-filter="branches" role="menu">

        <div data-filterable-for="context-commitish-filter-field" data-filterable-type="substring">


            <a class="select-menu-item js-navigation-item js-navigation-open selected"
               href="/GeniusVJR/LearningNotes/blob/master/Part2/JavaSE/Java%E5%9F%BA%E7%A1%80%E7%9F%A5%E8%AF%86.md"
               data-name="master"
               data-skip-pjax="true"
               rel="nofollow">
              <svg aria-hidden="true" class="octicon octicon-check select-menu-item-icon" height="16" version="1.1" viewBox="0 0 12 16" width="12"><path d="M12 5l-8 8-4-4 1.5-1.5L4 10l6.5-6.5z"></path></svg>
              <span class="select-menu-item-text css-truncate-target js-select-menu-filter-text">
                master
              </span>
            </a>
        </div>

          <div class="select-menu-no-results">Nothing to show</div>
      </div>

      <div class="select-menu-list select-menu-tab-bucket js-select-menu-tab-bucket" data-tab-filter="tags">
        <div data-filterable-for="context-commitish-filter-field" data-filterable-type="substring">


        </div>

        <div class="select-menu-no-results">Nothing to show</div>
      </div>

    </div>
  </div>
</div>

  <div class="BtnGroup float-right">
    <a href="/GeniusVJR/LearningNotes/find/master"
          class="js-pjax-capture-input btn btn-sm BtnGroup-item"
          data-pjax
          data-hotkey="t">
      Find file
    </a>
    <button aria-label="Copy file path to clipboard" class="js-zeroclipboard btn btn-sm BtnGroup-item tooltipped tooltipped-s" data-copied-hint="Copied!" type="button">Copy path</button>
  </div>
  <div class="breadcrumb js-zeroclipboard-target">
    <span class="repo-root js-repo-root"><span class="js-path-segment"><a href="/GeniusVJR/LearningNotes"><span>LearningNotes</span></a></span></span><span class="separator">/</span><span class="js-path-segment"><a href="/GeniusVJR/LearningNotes/tree/master/Part2"><span>Part2</span></a></span><span class="separator">/</span><span class="js-path-segment"><a href="/GeniusVJR/LearningNotes/tree/master/Part2/JavaSE"><span>JavaSE</span></a></span><span class="separator">/</span><strong class="final-path">Java基础知识.md</strong>
  </div>
</div>


  <div class="commit-tease">
      <span class="float-right">
        <a class="commit-tease-sha" href="/GeniusVJR/LearningNotes/commit/ebb6e865785cde22b97b553c40a4dc7e14c4e278" data-pjax>
          ebb6e86
        </a>
        <relative-time datetime="2016-10-21T15:05:43Z">Oct 21, 2016</relative-time>
      </span>
      <div>
        <img alt="@akuma" class="avatar" height="20" src="https://avatars0.githubusercontent.com/u/237677?v=3&amp;s=40" width="20" />
        <a href="/akuma" class="user-mention" rel="contributor">akuma</a>
          <a href="/GeniusVJR/LearningNotes/commit/ebb6e865785cde22b97b553c40a4dc7e14c4e278" class="message" data-pjax="true" title="Update Java基础知识.md">Update Java基础知识.md</a>
      </div>

    <div class="commit-tease-contributors">
      <button type="button" class="btn-link muted-link contributors-toggle" data-facebox="#blob_contributors_box">
        <strong>3</strong>
         contributors
      </button>
          <a class="avatar-link tooltipped tooltipped-s" aria-label="anAngryAnt" href="/GeniusVJR/LearningNotes/commits/master/Part2/JavaSE/Java%E5%9F%BA%E7%A1%80%E7%9F%A5%E8%AF%86.md?author=anAngryAnt"><img alt="@anAngryAnt" class="avatar" height="20" src="https://avatars2.githubusercontent.com/u/11955967?v=3&amp;s=40" width="20" /> </a>
    <a class="avatar-link tooltipped tooltipped-s" aria-label="GeniusVJR" href="/GeniusVJR/LearningNotes/commits/master/Part2/JavaSE/Java%E5%9F%BA%E7%A1%80%E7%9F%A5%E8%AF%86.md?author=GeniusVJR"><img alt="@GeniusVJR" class="avatar" height="20" src="https://avatars2.githubusercontent.com/u/13393725?v=3&amp;s=40" width="20" /> </a>
    <a class="avatar-link tooltipped tooltipped-s" aria-label="akuma" href="/GeniusVJR/LearningNotes/commits/master/Part2/JavaSE/Java%E5%9F%BA%E7%A1%80%E7%9F%A5%E8%AF%86.md?author=akuma"><img alt="@akuma" class="avatar" height="20" src="https://avatars0.githubusercontent.com/u/237677?v=3&amp;s=40" width="20" /> </a>


    </div>

    <div id="blob_contributors_box" style="display:none">
      <h2 class="facebox-header" data-facebox-id="facebox-header">Users who have contributed to this file</h2>
      <ul class="facebox-user-list" data-facebox-id="facebox-description">
          <li class="facebox-user-list-item">
            <img alt="@anAngryAnt" height="24" src="https://avatars0.githubusercontent.com/u/11955967?v=3&amp;s=48" width="24" />
            <a href="/anAngryAnt">anAngryAnt</a>
          </li>
          <li class="facebox-user-list-item">
            <img alt="@GeniusVJR" height="24" src="https://avatars0.githubusercontent.com/u/13393725?v=3&amp;s=48" width="24" />
            <a href="/GeniusVJR">GeniusVJR</a>
          </li>
          <li class="facebox-user-list-item">
            <img alt="@akuma" height="24" src="https://avatars2.githubusercontent.com/u/237677?v=3&amp;s=48" width="24" />
            <a href="/akuma">akuma</a>
          </li>
      </ul>
    </div>
  </div>

<div class="file">
  <div class="file-header">
  <div class="file-actions">

    <div class="BtnGroup">
      <a href="/GeniusVJR/LearningNotes/raw/master/Part2/JavaSE/Java%E5%9F%BA%E7%A1%80%E7%9F%A5%E8%AF%86.md" class="btn btn-sm BtnGroup-item" id="raw-url">Raw</a>
        <a href="/GeniusVJR/LearningNotes/blame/master/Part2/JavaSE/Java%E5%9F%BA%E7%A1%80%E7%9F%A5%E8%AF%86.md" class="btn btn-sm js-update-url-with-hash BtnGroup-item">Blame</a>
      <a href="/GeniusVJR/LearningNotes/commits/master/Part2/JavaSE/Java%E5%9F%BA%E7%A1%80%E7%9F%A5%E8%AF%86.md" class="btn btn-sm BtnGroup-item" rel="nofollow">History</a>
    </div>

        <a class="btn-octicon tooltipped tooltipped-nw"
           href="https://windows.github.com"
           aria-label="Open this file in GitHub Desktop"
           data-ga-click="Repository, open with desktop, type:windows">
            <svg aria-hidden="true" class="octicon octicon-device-desktop" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path d="M15 2H1c-.55 0-1 .45-1 1v9c0 .55.45 1 1 1h5.34c-.25.61-.86 1.39-2.34 2h8c-1.48-.61-2.09-1.39-2.34-2H15c.55 0 1-.45 1-1V3c0-.55-.45-1-1-1zm0 9H1V3h14v8z"></path></svg>
        </a>

        <!-- '"` --><!-- </textarea></xmp> --></option></form><form accept-charset="UTF-8" action="/GeniusVJR/LearningNotes/edit/master/Part2/JavaSE/Java%E5%9F%BA%E7%A1%80%E7%9F%A5%E8%AF%86.md" class="inline-form js-update-url-with-hash" data-form-nonce="ac627e2bd3e01a6c163de6f861a275d912e8c9c6" method="post"><div style="margin:0;padding:0;display:inline"><input name="utf8" type="hidden" value="&#x2713;" /><input name="authenticity_token" type="hidden" value="lsFpcej1P3UwOZQMDTC7gjK5SqYRUp2BPneCTJOLvnJljXFr1Mu07BixmqEGOdgCidh1MG0PCrfHFRpmMQ5YrA==" /></div>
          <button class="btn-octicon tooltipped tooltipped-nw" type="submit"
            aria-label="Fork this project and edit the file" data-hotkey="e" data-disable-with>
            <svg aria-hidden="true" class="octicon octicon-pencil" height="16" version="1.1" viewBox="0 0 14 16" width="14"><path d="M0 12v3h3l8-8-3-3-8 8zm3 2H1v-2h1v1h1v1zm10.3-9.3L12 6 9 3l1.3-1.3a.996.996 0 0 1 1.41 0l1.59 1.59c.39.39.39 1.02 0 1.41z"></path></svg>
          </button>
</form>        <!-- '"` --><!-- </textarea></xmp> --></option></form><form accept-charset="UTF-8" action="/GeniusVJR/LearningNotes/delete/master/Part2/JavaSE/Java%E5%9F%BA%E7%A1%80%E7%9F%A5%E8%AF%86.md" class="inline-form" data-form-nonce="ac627e2bd3e01a6c163de6f861a275d912e8c9c6" method="post"><div style="margin:0;padding:0;display:inline"><input name="utf8" type="hidden" value="&#x2713;" /><input name="authenticity_token" type="hidden" value="liCzB/rzdcaDvksEaXPxfb/Uk5CtC44hEKUJLewAEIfRrlttkQlOEtxDfx6xHAi0KTeh86ZVj0w/GNHxtr3yKQ==" /></div>
          <button class="btn-octicon btn-octicon-danger tooltipped tooltipped-nw" type="submit"
            aria-label="Fork this project and delete the file" data-disable-with>
            <svg aria-hidden="true" class="octicon octicon-trashcan" height="16" version="1.1" viewBox="0 0 12 16" width="12"><path d="M11 2H9c0-.55-.45-1-1-1H5c-.55 0-1 .45-1 1H2c-.55 0-1 .45-1 1v1c0 .55.45 1 1 1v9c0 .55.45 1 1 1h7c.55 0 1-.45 1-1V5c.55 0 1-.45 1-1V3c0-.55-.45-1-1-1zm-1 12H3V5h1v8h1V5h1v8h1V5h1v8h1V5h1v9zm1-10H2V3h9v1z"></path></svg>
          </button>
</form>  </div>

  <div class="file-info">
      545 lines (315 sloc)
      <span class="file-info-divider"></span>
    33.3 KB
  </div>
</div>

  
  <div id="readme" class="readme blob instapaper_body">
    <article class="markdown-body entry-content" itemprop="text"><h1><a id="user-content-j2se" class="anchor" href="#j2se" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>J2SE</h1>

<hr>

<h2><a id="user-content-基础" class="anchor" href="#基础" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>基础</h2>

<hr>

<p><strong>八种基本数据类型的大小，以及他们的封装类。</strong></p>

<p>八种基本数据类型，int ,double ,long ,float, short,byte,character,boolean</p>

<p>对应的封装类型是：Integer ,Double ,Long ,Float, Short,Byte,Character,Boolean</p>

<hr>

<p><strong>Switch能否用string做参数？</strong></p>

<p>在Java 5以前，switch(expr)中，expr只能是byte、short、char、int。从Java 5开始，Java中引入了枚举类型，expr也可以是enum类型，从Java 7开始，expr还可以是字符串（String），但是长整型（long）在目前所有的版本中都是不可以的。</p>

<hr>

<p><strong>equals与==的区别。</strong></p>

<p><a href="http://www.importnew.com/6804.html">http://www.importnew.com/6804.html</a></p>

<blockquote>
<p>==与equals的主要区别是：==常用于比较原生类型，而equals()方法用于检查对象的相等性。另一个不同的点是：如果==和equals()用于比较对象，当两个引用地址相同，==返回true。而equals()可以返回true或者false主要取决于重写实现。最常见的一个例子，字符串的比较，不同情况==和equals()返回不同的结果。equals()方法最重要的一点是，能够根据业务要求去重写，按照自定义规则去判断两个对象是否相等。重写equals()方法的时候，要注意一下hashCode是否会因为对象的属性改变而改变，否则在使用散列集合储存该对象的时候会碰到坑！！理解equals()方法的存在是很重要的。</p>
</blockquote>

<ol>
<li><p>使用==比较有两种情况：</p>

<pre><code>比较基础数据类型(Java中基础数据类型包括八中：short,int,long,float,double,char,byte,boolen)：这种情况下，==比较的是他们的值是否相等。
引用间的比较：在这种情况下，==比较的是他们在内存中的地址，也就是说，除非引用指向的是同一个new出来的对象，此时他们使用`==`去比较得到true，否则，得到false。
</code></pre></li>
<li><p>使用equals进行比较：</p>

<pre><code>equals追根溯源，是Object类中的一个方法，在该类中，equals的实现也仅仅只是比较两个对象的内存地址是否相等，但在一些子类中，如：String、Integer 等，该方法将被重写。
</code></pre></li>
<li><p>以<code>String</code>类为例子说明<code>eqauls</code>与<code>==</code>的区别：</p>

<blockquote>
<p>在开始这个例子之前，同学们需要知道JVM处理String的一些特性。<em>Java的虚拟机在内存中开辟出一块单独的区域，用来存储字符串对象，这块内存区域被称为字符串缓冲池。</em>当使用
<code>String a = "abc"</code>这样的语句进行定义一个引用的时候，首先会在<em>字符串缓冲池</em>中查找是否已经相同的对象，如果存在，那么就直接将这个对象的引用返回给a，如果不存在，则需要新建一个值为"abc"的对象，再将新的引用返回a。<code>String a = new String("abc");</code>这样的语句明确告诉JVM想要产生一个新的String对象，并且值为"abc"，于是就<em>在堆内存中的某一个小角落开辟了一个新的String对象</em>。</p>
</blockquote>

<ul>
<li><code>==</code>在比较引用的情况下，会去比较两个引用的内存地址是否相等。</li>
</ul>

<pre><code>    String str1 = "abc";
    String str2 = "abc";

    System.out.println(str1 == str2);
    System.out.println(str1.equals(str2));

    String str2 = new String("abc");
    System.out.println(str1 == str2);
    System.out.println(str1.equals(str2));

</code></pre>

<pre><code>以上代码将会输出
true
true
false
true
**第一个true：**因为在str2赋值之前，str1的赋值操作就已经在内存中创建了一个值为"abc"的对象了，然后str2将会与str1指向相同的地址。
**第二个true：**因为`String`已经重写了`equals`方法：为了方便大家阅读我贴出来，并且在注释用进行分析：
```
public boolean equals(Object anObject) {
//如果比较的对象与自身内存地址相等的话
//就说明他两指向的是同一个对象
//所以此时equals的返回值跟==的结果是一样的。
if (this == anObject) {
    return true;
}
//当比较的对象与自身的内存地址不相等，并且
//比较的对象是String类型的时候
//将会执行这个分支
if (anObject instanceof String) {
    String anotherString = (String)anObject;
    int n = value.length;
    if (n == anotherString.value.length) {
        char v1[] = value;
        char v2[] = anotherString.value;
        int i = 0;
        //在这里循环遍历两个String中的char
        while (n-- != 0) {
            //只要有一个不相等，那么就会返回false
            if (v1[i] != v2[i])
                return false;
            i++;
        }
        return true;
    }
}
return false;
</code></pre>

<p>}
    ```
    进行以上分析之后，就不难理解第一段代码中的实例程序输出了。</p></li>
</ol>

<hr>

<p><strong>Object有哪些公用方法？</strong></p>

<p><a href="http://www.cnblogs.com/yumo/p/4908315.html">http://www.cnblogs.com/yumo/p/4908315.html</a></p>

<p>1．clone方法</p>

<p>保护方法，实现对象的浅复制，只有实现了Cloneable接口才可以调用该方法，否则抛出CloneNotSupportedException异常。</p>

<p>主要是JAVA里除了8种基本类型传参数是值传递，其他的类对象传参数都是引用传递，我们有时候不希望在方法里讲参数改变，这是就需要在类中复写clone方法。</p>

<p>2．getClass方法</p>

<p>final方法，获得运行时类型。</p>

<p>3．toString方法</p>

<p>该方法用得比较多，一般子类都有覆盖。</p>

<p>4．finalize方法</p>

<p>该方法用于释放资源。因为无法确定该方法什么时候被调用，很少使用。</p>

<p>5．equals方法</p>

<p>该方法是非常重要的一个方法。一般equals和==是不一样的，但是在Object中两者是一样的。子类一般都要重写这个方法。</p>

<p>6．hashCode方法</p>

<p>该方法用于哈希查找，可以减少在查找中使用equals的次数，重写了equals方法一般都要重写hashCode方法。这个方法在一些具有哈希功能的Collection中用到。</p>

<p>一般必须满足obj1.equals(obj2)==true。可以推出obj1.hashCode()==obj2.hashCode()，但是hashCode相等不一定就满足equals。不过为了提高效率，应该尽量使上面两个条件接近等价。</p>

<p>如果不重写hashCode(),在HashSet中添加两个equals的对象，会将两个对象都加入进去。</p>

<p>7．wait方法</p>

<p>wait方法就是使当前线程等待该对象的锁，当前线程必须是该对象的拥有者，也就是具有该对象的锁。wait()方法一直等待，直到获得锁或者被中断。wait(long timeout)设定一个超时间隔，如果在规定时间内没有获得锁就返回。</p>

<p>调用该方法后当前线程进入睡眠状态，直到以下事件发生。</p>

<p>（1）其他线程调用了该对象的notify方法。</p>

<p>（2）其他线程调用了该对象的notifyAll方法。</p>

<p>（3）其他线程调用了interrupt中断该线程。</p>

<p>（4）时间间隔到了。</p>

<p>此时该线程就可以被调度了，如果是被中断的话就抛出一个InterruptedException异常。</p>

<p>8．notify方法</p>

<p>该方法唤醒在该对象上等待的某个线程。</p>

<p>9．notifyAll方法</p>

<p>该方法唤醒在该对象上等待的所有线程。</p>

<hr>

<p><strong>Java的四种引用，强弱软虚，用到的场景。</strong></p>

<p>JDK1.2之前只有强引用,其他几种引用都是在JDK1.2之后引入的.</p>

<ul>
<li><p>强引用（Strong Reference）
最常用的引用类型，如Object obj = new Object(); 。只要强引用存在则GC时则必定不被回收。</p></li>
<li><p>软引用（Soft Reference）
用于描述还有用但非必须的对象，当堆将发生OOM（Out Of Memory）时则会回收软引用所指向的内存空间，若回收后依然空间不足才会抛出OOM。一般用于实现内存敏感的高速缓存。
当真正对象被标记finalizable以及的finalize()方法调用之后并且内存已经清理, 那么如果SoftReference object还存在就被加入到它的 ReferenceQueue.只有前面几步完成后,Soft Reference和Weak Reference的get方法才会返回null</p></li>
<li><p>弱引用（Weak Reference）
发生GC时必定回收弱引用指向的内存空间。
和软引用加入队列的时机相同</p></li>
<li><p>虚引用（Phantom Reference)
又称为幽灵引用或幻影引用，虚引用既不会影响对象的生命周期，也无法通过虚引用来获取对象实例，仅用于在发生GC时接收一个系统通知。
当一个对象的finalize方法已经被调用了之后，这个对象的幽灵引用会被加入到队列中。通过检查该队列里面的内容就知道一个对象是不是已经准备要被回收了.
虚引用和软引用和弱引用都不同,它会在内存没有清理的时候被加入引用队列.虚引用的建立必须要传入引用队列,其他可以没有</p></li>
</ul>

<hr>

<p><strong>Hashcode的作用。</strong></p>

<p><a href="http://c610367182.iteye.com/blog/1930676">http://c610367182.iteye.com/blog/1930676</a></p>

<p>以Java.lang.Object来理解,JVM每new一个Object,它都会将这个Object丢到一个Hash哈希表中去,这样的话,下次做Object的比较或者取这个对象的时候,它会根据对象的hashcode再从Hash表中取这个对象。这样做的目的是提高取对象的效率。具体过程是这样: </p>

<ol>
<li><p>new Object(),JVM根据这个对象的Hashcode值,放入到对应的Hash表对应的Key上,如果不同的对象确产生了相同的hash值,也就是发生了Hash key相同导致冲突的情况,那么就在这个Hash key的地方产生一个链表,将所有产生相同hashcode的对象放到这个单链表上去,串在一起。 </p></li>
<li><p>比较两个对象的时候,首先根据他们的hashcode去hash表中找他的对象,当两个对象的hashcode相同,那么就是说他们这两个对象放在Hash表中的同一个key上,那么他们一定在这个key上的链表上。那么此时就只能根据Object的equal方法来比较这个对象是否equal。当两个对象的hashcode不同的话，肯定他们不能equal. </p></li>
</ol>

<hr>

<p><strong>String、StringBuffer与StringBuilder的区别。</strong></p>

<p>Java 平台提供了两种类型的字符串：String和StringBuffer / StringBuilder，它们可以储存和操作字符串。其中String是只读字符串，也就意味着String引用的字符串内容是不能被改变的。而StringBuffer和StringBulder类表示的字符串对象可以直接进行修改。StringBuilder是JDK1.5引入的，它和StringBuffer的方法完全相同，区别在于它是单线程环境下使用的，因为它的所有方面都没有被synchronized修饰，因此它的效率也比StringBuffer略高。</p>

<hr>

<p><strong>try catch finally，try里有return，finally还执行么？</strong></p>

<p>会执行，在方法 返回调用者前执行。Java允许在finally中改变返回值的做法是不好的，因为如果存在finally代码块，try中的return语句不会立马返回调用者，而是纪录下返回值待finally代码块执行完毕之后再向调用者返回其值，然后如果在finally中修改了返回值，这会对程序造成很大的困扰，C#中就从语法规定不能做这样的事。</p>

<hr>

<p><strong>Excption与Error区别</strong></p>

<p>Error表示系统级的错误和程序不必处理的异常，是恢复不是不可能但很困难的情况下的一种严重问题；比如内存溢出，不可能指望程序能处理这样的状况；Exception表示需要捕捉或者需要程序进行处理的异常，是一种设计或实现问题；也就是说，它表示如果程序运行正常，从不会发生的情况。</p>

<hr>

<p><strong>Excption与Error包结构。OOM你遇到过哪些情况，SOF你遇到过哪些情况。</strong></p>

<p><a href="http://www.cnblogs.com/yumo/p/4909617.html">http://www.cnblogs.com/yumo/p/4909617.html</a></p>

<p>Java异常架构图</p>

<p><a href="https://camo.githubusercontent.com/2248cdf95b8f2569ee0e58aac3d8ed179c89f190/687474703a2f2f696d61676573323031352e636e626c6f67732e636f6d2f626c6f672f3637393930342f3230313531302f3637393930342d32303135313032353231303831333938392d3932313932373931362e6a7067" target="_blank"><img src="https://camo.githubusercontent.com/2248cdf95b8f2569ee0e58aac3d8ed179c89f190/687474703a2f2f696d61676573323031352e636e626c6f67732e636f6d2f626c6f672f3637393930342f3230313531302f3637393930342d32303135313032353231303831333938392d3932313932373931362e6a7067" alt="" data-canonical-src="http://images2015.cnblogs.com/blog/679904/201510/679904-20151025210813989-921927916.jpg" style="max-width:100%;"></a></p>

<ol>
<li><p>Throwable 
Throwable是 Java 语言中所有错误或异常的超类。 
Throwable包含两个子类: Error 和 Exception 。它们通常用于指示发生了异常情况。 
Throwable包含了其线程创建时线程执行堆栈的快照，它提供了printStackTrace()等接口用于获取堆栈跟踪数据等信息。</p></li>
<li><p>Exception 
Exception及其子类是 Throwable 的一种形式，它指出了合理的应用程序想要捕获的条件。</p></li>
<li><p>RuntimeException 
RuntimeException是那些可能在 Java 虚拟机正常运行期间抛出的异常的超类。 
编译器不会检查RuntimeException异常。 例如，除数为零时，抛出ArithmeticException异常。RuntimeException是ArithmeticException的超类。当代码发生除数为零的情况时，倘若既"没有通过throws声明抛出ArithmeticException异常"，也"没有通过try...catch...处理该异常"，也能通过编译。这就是我们所说的"编译器不会检查RuntimeException异常"！ 
如果代码会产生RuntimeException异常，则需要通过修改代码进行避免。 例如，若会发生除数为零的情况，则需要通过代码避免该情况的发生！</p></li>
<li><p>Error 
和Exception一样， Error也是Throwable的子类。 它用于指示合理的应用程序不应该试图捕获的严重问题，大多数这样的错误都是异常条件。 
和RuntimeException一样， 编译器也不会检查Error。</p></li>
</ol>

<p>Java将可抛出(Throwable)的结构分为三种类型： 被检查的异常(Checked Exception)，运行时异常(RuntimeException)和错误(Error)。</p>

<p>(01) 运行时异常 
定义 : RuntimeException及其子类都被称为运行时异常。 
特点 : Java编译器不会检查它。 也就是说，当程序中可能出现这类异常时，倘若既"没有通过throws声明抛出它"，也"没有用try-catch语句捕获它"，还是会编译通过。例如，除数为零时产生的ArithmeticException异常，数组越界时产生的IndexOutOfBoundsException异常，fail-fail机制产生的ConcurrentModificationException异常等，都属于运行时异常。 
虽然Java编译器不会检查运行时异常，但是我们也可以通过throws进行声明抛出，也可以通过try-catch对它进行捕获处理。 
如果产生运行时异常，则需要通过修改代码来进行避免。 例如，若会发生除数为零的情况，则需要通过代码避免该情况的发生！</p>

<p>(02) 被检查的异常 
定义 :  Exception类本身，以及Exception的子类中除了"运行时异常"之外的其它子类都属于被检查异常。 
特点 : Java编译器会检查它。 此类异常，要么通过throws进行声明抛出，要么通过try-catch进行捕获处理，否则不能通过编译。例如，CloneNotSupportedException就属于被检查异常。当通过clone()接口去克隆一个对象，而该对象对应的类没有实现Cloneable接口，就会抛出CloneNotSupportedException异常。 
被检查异常通常都是可以恢复的。</p>

<p>(03) 错误 
定义 : Error类及其子类。 
特点 : 和运行时异常一样，编译器也不会对错误进行检查。 
当资源不足、约束失败、或是其它程序无法继续运行的条件发生时，就产生错误。程序本身无法修复这些错误的。例如，VirtualMachineError就属于错误。 
按照Java惯例，我们是不应该是实现任何新的Error子类的！</p>

<p>对于上面的3种结构，我们在抛出异常或错误时，到底该哪一种？《Effective Java》中给出的建议是： 对于可以恢复的条件使用被检查异常，对于程序错误使用运行时异常。</p>

<hr>

<p><strong>OOM：</strong></p>

<ol>
<li><p>OutOfMemoryError异常</p>

<p>除了程序计数器外，虚拟机内存的其他几个运行时区域都有发生OutOfMemoryError(OOM)异常的可能，</p>

<p>Java Heap 溢出</p>

<p>一般的异常信息：java.lang.OutOfMemoryError:Java heap spacess</p>

<p>java堆用于存储对象实例，我们只要不断的创建对象，并且保证GC Roots到对象之间有可达路径来避免垃圾回收机制清除这些对象，就会在对象数量达到最大堆容量限制后产生内存溢出异常。</p>

<p>出现这种异常，一般手段是先通过内存映像分析工具(如Eclipse Memory Analyzer)对dump出来的堆转存快照进行分析，重点是确认内存中的对象是否是必要的，先分清是因为内存泄漏(Memory Leak)还是内存溢出(Memory Overflow)。</p>

<p>如果是内存泄漏，可进一步通过工具查看泄漏对象到GC Roots的引用链。于是就能找到泄漏对象时通过怎样的路径与GC Roots相关联并导致垃圾收集器无法自动回收。</p>

<p>如果不存在泄漏，那就应该检查虚拟机的参数(-Xmx与-Xms)的设置是否适当。</p></li>
<li><p>虚拟机栈和本地方法栈溢出</p>

<p>如果线程请求的栈深度大于虚拟机所允许的最大深度，将抛出StackOverflowError异常。</p>

<p>如果虚拟机在扩展栈时无法申请到足够的内存空间，则抛出OutOfMemoryError异常</p>

<p>这里需要注意当栈的大小越大可分配的线程数就越少。</p></li>
<li><p>运行时常量池溢出</p>

<p>异常信息：java.lang.OutOfMemoryError:PermGen space</p>

<p>如果要向运行时常量池中添加内容，最简单的做法就是使用String.intern()这个Native方法。该方法的作用是：如果池中已经包含一个等于此String的字符串，则返回代表池中这个字符串的String对象；否则，将此String对象包含的字符串添加到常量池中，并且返回此String对象的引用。由于常量池分配在方法区内，我们可以通过-XX:PermSize和-XX:MaxPermSize限制方法区的大小，从而间接限制其中常量池的容量。</p></li>
<li><p>方法区溢出</p>

<p>方法区用于存放Class的相关信息，如类名、访问修饰符、常量池、字段描述、方法描述等。</p>

<p>异常信息：java.lang.OutOfMemoryError:PermGen space</p>

<p>方法区溢出也是一种常见的内存溢出异常，一个类如果要被垃圾收集器回收，判定条件是很苛刻的。在经常动态生成大量Class的应用中，要特别注意这点。</p></li>
</ol>

<hr>

<p><strong>Java面向对象的三个特征与含义。</strong></p>

<p>继承：继承是从已有类得到继承信息创建新类的过程。提供继承信息的类被称为父类（超类、基类）；得到继承信息的类被称为子类（派生类）。继承让变化中的软件系统有了一定的延续性，同时继承也是封装程序中可变因素的重要手段。</p>

<p>封装：通常认为封装是把数据和操作数据的方法绑定起来，对数据的访问只能通过已定义的接口。面向对象的本质就是将现实世界描绘成一系列完全自治、封闭的对象。我们在类中编写的方法就是对实现细节的一种封装；我们编写一个类就是对数据和数据操作的封装。可以说，封装就是隐藏一切可隐藏的东西，只向外界提供最简单的编程接口（可以想想普通洗衣机和全自动洗衣机的差别，明显全自动洗衣机封装更好因此操作起来更简单；我们现在使用的智能手机也是封装得足够好的，因为几个按键就搞定了所有的事情）。</p>

<p>多态：多态性是指允许不同子类型的对象对同一消息作出不同的响应。简单的说就是用同样的对象引用调用同样的方法但是做了不同的事情。多态性分为编译时的多态性和运行时的多态性。如果将对象的方法视为对象向外界提供的服务，那么运行时的多态性可以解释为：当A系统访问B系统提供的服务时，B系统有多种提供服务的方式，但一切对A系统来说都是透明的（就像电动剃须刀是A系统，它的供电系统是B系统，B系统可以使用电池供电或者用交流电，甚至还有可能是太阳能，A系统只会通过B类对象调用供电的方法，但并不知道供电系统的底层实现是什么，究竟通过何种方式获得了动力）。方法重载（overload）实现的是编译时的多态性（也称为前绑定），而方法重写（override）实现的是运行时的多态性（也称为后绑定）。运行时的多态是面向对象最精髓的东西，要实现多态需要做两件事：1. 方法重写（子类继承父类并重写父类中已有的或抽象的方法）；2. 对象造型（用父类型引用引用子类型对象，这样同样的引用调用同样的方法就会根据子类对象的不同而表现出不同的行为）。</p>

<hr>

<p><strong>Override和Overload的含义与区别。</strong></p>

<p>Overload：顾名思义，就是Over(重新)——load（加载），所以中文名称是重载。它可以表现类的多态性，可以是函数里面可以有相同的函数名但是参数名、类型不能相同；或者说可以改变参数、类型但是函数名字依然不变。</p>

<p>Override：就是ride(重写)的意思，在子类继承父类的时候子类中可以定义某方法与其父类有相同的名称和参数，当子类在调用这一函数时自动调用子类的方法，而父类相当于被覆盖（重写）了。</p>

<p>方法的重写Overriding和重载Overloading是Java多态性的不同表现。重写Overriding是父类与子类之间多态性的一种表现，重载Overloading是一个类中多态性的一种表现。如果在子类中定义某方法与其父类有相同的名称和参数，我们说该方法被重写 (Overriding)。子类的对象使用这个方法时，将调用子类中的定义，对它而言，父类中的定义如同被“屏蔽”了。如果在一个类中定义了多个同名的方法，它们或有不同的参数个数或有不同的参数类型，则称为方法的重载(Overloading)。Overloaded的方法是可以改变返回值的类型。</p>

<hr>

<p><strong>Interface与abstract类的区别。</strong></p>

<p>抽象类和接口都不能够实例化，但可以定义抽象类和接口类型的引用。一个类如果继承了某个抽象类或者实现了某个接口都需要对其中的抽象方法全部进行实现，否则该类仍然需要被声明为抽象类。接口比抽象类更加抽象，因为抽象类中可以定义构造器，可以有抽象方法和具体方法，而接口中不能定义构造器而且其中的方法全部都是抽象方法。抽象类中的成员可以是private、默认、protected、public的，而接口中的成员全都是public的。抽象类中可以定义成员变量，而接口中定义的成员变量实际上都是常量。有抽象方法的类必须被声明为抽象类，而抽象类未必要有抽象方法。</p>

<hr>

<p><strong>Static class 与non static class的区别。</strong></p>

<p>内部静态类不需要有指向外部类的引用。但非静态内部类需要持有对外部类的引用。非静态内部类能够访问外部类的静态和非静态成员。静态类不能访问外部类的非静态成员。他只能访问外部类的静态成员。一个非静态内部类不能脱离外部类实体被创建，一个非静态内部类可以访问外部类的数据和方法，因为他就在外部类里面。</p>

<hr>

<p><strong>java多态的实现原理。</strong></p>

<p><a href="http://blog.csdn.net/zzzhangzhun/article/details/51095075">http://blog.csdn.net/zzzhangzhun/article/details/51095075</a></p>

<p>当JVM执行Java字节码时，类型信息会存储在方法区中，为了优化对象的调用方法的速度，方法区的类型信息会增加一个指针，该指针指向一个记录该类方法的方法表，方法表中的每一个项都是对应方法的指针。</p>

<p>方法区：方法区和JAVA堆一样，是各个线程共享的内存区域，用于存储已被虚拟机加载的类信息、常量、静态变量、即时编译器编译后的代码等数据。 
运行时常量池：它是方法区的一部分，Class文件中除了有类的版本、方法、字段等描述信息外，还有一项信息是常量池，用于存放编译器生成的各种符号引用，这部分信息在类加载时进入方法区的运行时常量池中。 
方法区的内存回收目标是针对常量池的回收及对类型的卸载。</p>

<p>方法表的构造</p>

<p>由于java的单继承机制，一个类只能继承一个父类，而所有的类又都继承Object类，方法表中最先存放的是Object的方法，接下来是父类的方法，最后是该类本身的方法。如果子类改写了父类的方法，那么子类和父类的那些同名的方法共享一个方法表项。</p>

<p>由于这样的特性，使得方法表的偏移量总是固定的，例如，对于任何类来说，其方法表的equals方法的偏移量总是一个定值，所有继承父类的子类的方法表中，其父类所定义的方法的偏移量也总是一个定值。</p>

<p>实例</p>

<p>假设Class A是Class B的子类，并且A改写了B的方法的method()，那么B来说，method方法的指针指向B的method方法入口；对于A来说，A的方法表的method项指向自身的method而非父类的。</p>

<p>流程：调用方法时，虚拟机通过对象引用得到方法区中类型信息的方法表的指针入口，查询类的方法表 ，根据实例方法的符号引用解析出该方法在方法表的偏移量，子类对象声明为父类类型时，形式上调用的是父类的方法，此时虚拟机会从实际的方法表中找到方法地址，从而定位到实际类的方法。 
注：所有引用为父类，但方法区的类型信息中存放的是子类的信息，所以调用的是子类的方法表。</p>

<hr>

<p><strong>foreach与正常for循环效率对比。</strong></p>

<p><a href="http://904510742.iteye.com/blog/2118331">http://904510742.iteye.com/blog/2118331</a></p>

<p>直接for循环效率最高，其次是迭代器和 ForEach操作。
作为语法糖，其实 ForEach 编译成 字节码之后，使用的是迭代器实现的，反编译后，testForEach方法如下：</p>

<pre><code>public static void testForEach(List list) {  
    for (Iterator iterator = list.iterator(); iterator.hasNext();) {  
        Object t = iterator.next();  
        Object obj = t;  
    }  
}  
</code></pre>

<p>可以看到，只比迭代器遍历多了生成中间变量这一步，因为性能也略微下降了一些。</p>

<hr>

<p><strong>反射机制</strong></p>

<p>JAVA反射机制是在运行状态中, 对于任意一个类, 都能够知道这个类的所有属性和方法; 对于任意一个对象, 都能够调用它的任意一个方法和属性; 这种动态获取的信息以及动态调用对象的方法的功能称为java语言的反射机制.</p>

<p>主要作用有三：</p>

<p>运行时取得类的方法和字段的相关信息。</p>

<p>创建某个类的新实例(.newInstance())</p>

<p>取得字段引用直接获取和设置对象字段，无论访问修饰符是什么。</p>

<p>用处如下：</p>

<p>观察或操作应用程序的运行时行为。</p>

<p>调试或测试程序，因为可以直接访问方法、构造函数和成员字段。</p>

<p>通过名字调用不知道的方法并使用该信息来创建对象和调用方法。</p>

<hr>

<p><strong>String类内部实现，能否改变String对象内容</strong></p>

<p><a href="https://github.com/GeniusVJR/LearningNotes/blob/master/Part2/JavaSE/String%E6%BA%90%E7%A0%81%E5%88%86%E6%9E%90.md">String源码分析</a></p>

<p><a href="http://blog.csdn.net/zhangjg_blog/article/details/18319521">http://blog.csdn.net/zhangjg_blog/article/details/18319521</a></p>

<hr>

<p><strong>try catch 块，try里有return，finally也有return，如何执行</strong></p>

<p><a href="http://qing0991.blog.51cto.com/1640542/1387200">http://qing0991.blog.51cto.com/1640542/1387200</a></p>

<hr>

<p><strong>泛型的优缺点</strong></p>

<p>优点：</p>

<p>使用泛型类型可以最大限度地重用代码、保护类型的安全以及提高性能。</p>

<p>泛型最常见的用途是创建集合类。</p>

<p>缺点：</p>

<p>在性能上不如数组快。</p>

<hr>

<p><strong>泛型常用特点，List<code>&lt;String&gt;</code>能否转为List<code>&lt;Object&gt;</code></strong></p>

<p>能，但是利用类都继承自Object，所以使用是每次调用里面的函数都要通过强制转换还原回原来的类，这样既不安全，运行速度也慢。</p>

<hr>

<p><strong>解析XML的几种方式的原理与特点：DOM、SAX、PULL。</strong></p>

<p><a href="http://www.cnblogs.com/HaroldTihan/p/4316397.html">http://www.cnblogs.com/HaroldTihan/p/4316397.html</a></p>

<hr>

<p><strong>Java与C++对比。</strong></p>

<p><a href="http://developer.51cto.com/art/201106/270422.htm">http://developer.51cto.com/art/201106/270422.htm</a></p>

<hr>

<p><strong>Java1.7与1.8新特性。</strong></p>

<p><a href="http://blog.chinaunix.net/uid-29618857-id-4416835.html">http://blog.chinaunix.net/uid-29618857-id-4416835.html</a></p>

<hr>

<p><strong>JNI的使用。</strong></p>

<p><a href="http://landerlyoung.github.io/blog/2014/10/16/java-zhong-jnide-shi-yong/">http://landerlyoung.github.io/blog/2014/10/16/java-zhong-jnide-shi-yong/</a></p>

<hr>

<h3><a id="user-content-集合" class="anchor" href="#集合" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>集合</h3>

<p><strong>ArrayList、LinkedList、Vector的底层实现和区别</strong></p>

<ul>
<li>从同步性来看，ArrayList和LinkedList是不同步的，而Vector是的。所以线程安全的话，可以使用ArrayList或LinkedList，可以节省为同步而耗费的开销。但在多线程下，有时候就不得不使用Vector了。当然，也可以通过一些办法包装ArrayList、LinkedList，使我们也达到同步，但效率可能会有所降低。</li>
<li>从内部实现机制来讲ArrayList和Vector都是使用Object的数组形式来存储的。当你向这两种类型中增加元素的时候，如果元素的数目超出了内部数组目前的长度它们都需要扩展内部数组的长度，Vector缺省情况下自动增长原来一倍的数组长度，ArrayList是原来的50%，所以最后你获得的这个集合所占的空间总是比你实际需要的要大。如果你要在集合中保存大量的数据，那么使用Vector有一些优势，因为你可以通过设置集合的初始化大小来避免不必要的资源开销。</li>
<li>ArrayList和Vector中，从指定的位置（用index）检索一个对象，或在集合的末尾插入、删除一个对象的时间是一样的，可表示为O(1)。但是，如果在集合的其他位置增加或者删除元素那么花费的时间会呈线性增长O(n-i)，其中n代表集合中元素的个数，i代表元素增加或移除元素的索引位置，因为在进行上述操作的时候集合中第i和第i个元素之后的所有元素都要执行(n-i)个对象的位移操作。LinkedList底层是由双向循环链表实现的，LinkedList在插入、删除集合中任何位置的元素所花费的时间都是一样的O(1)，但它在索引一个元素的时候比较慢，为O(i)，其中i是索引的位置，如果只是查找特定位置的元素或只在集合的末端增加、移除元素，那么使用Vector或ArrayList都可以。如果是对其它指定位置的插入、删除操作，最好选择LinkedList。</li>
</ul>

<p><strong>HashMap和HashTable的底层实现和区别，两者和ConcurrentHashMap的区别。</strong></p>

<p><a href="http://blog.csdn.net/xuefeng0707/article/details/40834595">http://blog.csdn.net/xuefeng0707/article/details/40834595</a></p>

<p>HashTable线程安全则是依靠方法简单粗暴的sychronized修饰，HashMap则没有相关的线程安全问题考虑。。</p>

<p>在以前的版本貌似ConcurrentHashMap引入了一个“分段锁”的概念，具体可以理解为把一个大的Map拆分成N个小的HashTable，根据key.hashCode()来决定把key放到哪个HashTable中。在ConcurrentHashMap中，就是把Map分成了N个Segment，put和get的时候，都是现根据key.hashCode()算出放到哪个Segment中。</p>

<p>通过把整个Map分为N个Segment（类似HashTable），可以提供相同的线程安全，但是效率提升N倍。</p>

<hr>

<p><strong>HashMap的hashcode的作用？什么时候需要重写？如何解决哈希冲突？查找的时候流程是如何？</strong></p>

<p><a href="http://blog.csdn.net/codeemperor/article/details/51351247">从源码分析HashMap</a></p>

<hr>

<p><strong>Arraylist和HashMap如何扩容？负载因子有什么作用？如何保证读写进程安全？</strong></p>

<p><a href="http://m.blog.csdn.net/article/details?id=48956087">http://m.blog.csdn.net/article/details?id=48956087</a></p>

<p><a href="http://hovertree.com/h/bjaf/2jdr60li.htm">http://hovertree.com/h/bjaf/2jdr60li.htm</a></p>

<p>ArrayList 本身不是线程安全的。
所以正确的做法是去用 java.util.concurrent 里的 CopyOnWriteArrayList 或者某个同步的 Queue 类。</p>

<p>HashMap实现不是同步的。如果多个线程同时访问一个哈希映射，而其中至少一个线程从结构上修改了该映射，则它必须 保持外部同步。（结构上的修改是指添加或删除一个或多个映射关系的任何操作；仅改变与实例已经包含的键关联的值不是结构上的修改。）这一般通过对自然封装该映射的对象进行同步操作来完成。如果不存在这样的对象，则应该使用 Collections.synchronizedMap 方法来“包装”该映射。最好在创建时完成这一操作，以防止对映射进行意外的非同步访问.</p>

<hr>

<p><strong>TreeMap、HashMap、LinkedHashMap的底层实现区别。</strong></p>

<p><a href="http://blog.csdn.net/lolashe/article/details/20806319">http://blog.csdn.net/lolashe/article/details/20806319</a></p>

<hr>

<p><strong>Collection包结构，与Collections的区别。</strong></p>

<p>Collection是一个接口，它是Set、List等容器的父接口；Collections是一个工具类，提供了一系列的静态方法来辅助容器操作，这些方法包括对容器的搜索、排序、线程安全化等等。</p>

<hr>

<p><strong>Set、List之间的区别是什么?</strong></p>

<p><a href="http://developer.51cto.com/art/201309/410205_all.htm">http://developer.51cto.com/art/201309/410205_all.htm</a></p>

<hr>

<p><strong>Map、Set、List、Queue、Stack的特点与用法。</strong></p>

<p><a href="http://www.cnblogs.com/yumo/p/4908718.html">http://www.cnblogs.com/yumo/p/4908718.html</a></p>

<p>Collection 是对象集合， Collection 有两个子接口 List 和 Set</p>

<p>List 可以通过下标 (1,2..) 来取得值，值可以重复</p>

<p>而 Set 只能通过游标来取值，并且值是不能重复的</p>

<p>ArrayList ， Vector ， LinkedList 是 List 的实现类</p>

<p>ArrayList 是线程不安全的， Vector 是线程安全的，这两个类底层都是由数组实现的</p>

<p>LinkedList 是线程不安全的，底层是由链表实现的   </p>

<p>Map 是键值对集合</p>

<p>HashTable 和 HashMap 是 Map 的实现类<br>
HashTable 是线程安全的，不能存储 null 值<br>
HashMap 不是线程安全的，可以存储 null 值  </p>

<p>Stack类：继承自Vector，实现一个后进先出的栈。提供了几个基本方法，push、pop、peak、empty、search等。</p>

<p>Queue接口：提供了几个基本方法，offer、poll、peek等。已知实现类有LinkedList、PriorityQueue等。</p>
</article>
  </div>

</div>

<button type="button" data-facebox="#jump-to-line" data-facebox-class="linejump" data-hotkey="l" class="d-none">Jump to Line</button>
<div id="jump-to-line" style="display:none">
  <!-- '"` --><!-- </textarea></xmp> --></option></form><form accept-charset="UTF-8" action="" class="js-jump-to-line-form" method="get"><div style="margin:0;padding:0;display:inline"><input name="utf8" type="hidden" value="&#x2713;" /></div>
    <input class="form-control linejump-input js-jump-to-line-field" type="text" placeholder="Jump to line&hellip;" aria-label="Jump to line" autofocus>
    <button type="submit" class="btn">Go</button>
</form></div>

  </div>
  <div class="modal-backdrop js-touch-events"></div>
</div>


    </div>
  </div>

    </div>

        <div class="container site-footer-container">
  <div class="site-footer" role="contentinfo">
    <ul class="site-footer-links float-right">
        <li><a href="https://github.com/contact" data-ga-click="Footer, go to contact, text:contact">Contact GitHub</a></li>
      <li><a href="https://developer.github.com" data-ga-click="Footer, go to api, text:api">API</a></li>
      <li><a href="https://training.github.com" data-ga-click="Footer, go to training, text:training">Training</a></li>
      <li><a href="https://shop.github.com" data-ga-click="Footer, go to shop, text:shop">Shop</a></li>
        <li><a href="https://github.com/blog" data-ga-click="Footer, go to blog, text:blog">Blog</a></li>
        <li><a href="https://github.com/about" data-ga-click="Footer, go to about, text:about">About</a></li>

    </ul>

    <a href="https://github.com" aria-label="Homepage" class="site-footer-mark" title="GitHub">
      <svg aria-hidden="true" class="octicon octicon-mark-github" height="24" version="1.1" viewBox="0 0 16 16" width="24"><path d="M8 0C3.58 0 0 3.58 0 8c0 3.54 2.29 6.53 5.47 7.59.4.07.55-.17.55-.38 0-.19-.01-.82-.01-1.49-2.01.37-2.53-.49-2.69-.94-.09-.23-.48-.94-.82-1.13-.28-.15-.68-.52-.01-.53.63-.01 1.08.58 1.23.82.72 1.21 1.87.87 2.33.66.07-.52.28-.87.51-1.07-1.78-.2-3.64-.89-3.64-3.95 0-.87.31-1.59.82-2.15-.08-.2-.36-1.02.08-2.12 0 0 .67-.21 2.2.82.64-.18 1.32-.27 2-.27.68 0 1.36.09 2 .27 1.53-1.04 2.2-.82 2.2-.82.44 1.1.16 1.92.08 2.12.51.56.82 1.27.82 2.15 0 3.07-1.87 3.75-3.65 3.95.29.25.54.73.54 1.48 0 1.07-.01 1.93-.01 2.2 0 .21.15.46.55.38A8.013 8.013 0 0 0 16 8c0-4.42-3.58-8-8-8z"></path></svg>
</a>
    <ul class="site-footer-links">
      <li>&copy; 2016 <span title="0.12486s from github-fe126-cp1-prd.iad.github.net">GitHub</span>, Inc.</li>
        <li><a href="https://github.com/site/terms" data-ga-click="Footer, go to terms, text:terms">Terms</a></li>
        <li><a href="https://github.com/site/privacy" data-ga-click="Footer, go to privacy, text:privacy">Privacy</a></li>
        <li><a href="https://github.com/security" data-ga-click="Footer, go to security, text:security">Security</a></li>
        <li><a href="https://status.github.com/" data-ga-click="Footer, go to status, text:status">Status</a></li>
        <li><a href="https://help.github.com" data-ga-click="Footer, go to help, text:help">Help</a></li>
    </ul>
  </div>
</div>



    

    <div id="ajax-error-message" class="ajax-error-message flash flash-error">
      <svg aria-hidden="true" class="octicon octicon-alert" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path d="M8.865 1.52c-.18-.31-.51-.5-.87-.5s-.69.19-.87.5L.275 13.5c-.18.31-.18.69 0 1 .19.31.52.5.87.5h13.7c.36 0 .69-.19.86-.5.17-.31.18-.69.01-1L8.865 1.52zM8.995 13h-2v-2h2v2zm0-3h-2V6h2v4z"></path></svg>
      <button type="button" class="flash-close js-flash-close js-ajax-error-dismiss" aria-label="Dismiss error">
        <svg aria-hidden="true" class="octicon octicon-x" height="16" version="1.1" viewBox="0 0 12 16" width="12"><path d="M7.48 8l3.75 3.75-1.48 1.48L6 9.48l-3.75 3.75-1.48-1.48L4.52 8 .77 4.25l1.48-1.48L6 6.52l3.75-3.75 1.48 1.48z"></path></svg>
      </button>
      You can't perform that action at this time.
    </div>


      
      <script crossorigin="anonymous" integrity="sha256-NbnFQdNBMJuTCxx5D6GyejDHxEzhDH+CQokOPYPIrb0=" src="https://assets-cdn.github.com/assets/frameworks-35b9c541d341309b930b1c790fa1b27a30c7c44ce10c7f8242890e3d83c8adbd.js"></script>
      <script async="async" crossorigin="anonymous" integrity="sha256-KUc5sZMEhV0sUHfPRpDx7Im856pzqIhZt23B8iMWo9g=" src="https://assets-cdn.github.com/assets/github-294739b19304855d2c5077cf4690f1ec89bce7aa73a88859b76dc1f22316a3d8.js"></script>
      
      
      
      
    <div class="js-stale-session-flash stale-session-flash flash flash-warn flash-banner d-none">
      <svg aria-hidden="true" class="octicon octicon-alert" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path d="M8.865 1.52c-.18-.31-.51-.5-.87-.5s-.69.19-.87.5L.275 13.5c-.18.31-.18.69 0 1 .19.31.52.5.87.5h13.7c.36 0 .69-.19.86-.5.17-.31.18-.69.01-1L8.865 1.52zM8.995 13h-2v-2h2v2zm0-3h-2V6h2v4z"></path></svg>
      <span class="signed-in-tab-flash">You signed in with another tab or window. <a href="">Reload</a> to refresh your session.</span>
      <span class="signed-out-tab-flash">You signed out in another tab or window. <a href="">Reload</a> to refresh your session.</span>
    </div>
    <div class="facebox" id="facebox" style="display:none;">
  <div class="facebox-popup">
    <div class="facebox-content" role="dialog" aria-labelledby="facebox-header" aria-describedby="facebox-description">
    </div>
    <button type="button" class="facebox-close js-facebox-close" aria-label="Close modal">
      <svg aria-hidden="true" class="octicon octicon-x" height="16" version="1.1" viewBox="0 0 12 16" width="12"><path d="M7.48 8l3.75 3.75-1.48 1.48L6 9.48l-3.75 3.75-1.48-1.48L4.52 8 .77 4.25l1.48-1.48L6 6.52l3.75-3.75 1.48 1.48z"></path></svg>
    </button>
  </div>
</div>

  </body>
</html>

