# Atom Emmet extend configuration for bem
  I) How to configure Atom emmet package for extensions, such as defining the filter |bem always active. <br/>
  II) New bem filter syntax less confusing.
  
## I) Short story about preferences
  The procedure implied in the readme is really confusing and incomplete.
  Needed to read the END of the readme + doc https://docs.emmet.io/customization/ .<br/>
  You have to create choose the location and the name of the files you want yourself. <br/>
  This repo contains all the needed files with my preferences, modify them at your need.<br/>
  The preferences are split in three files "preferences.json", "snippets.json", "syntaxProfiles.json"
### I.1) Setup the preferences
  Place the Atom-emmet-extend-configuration-for-bem folder (rename it as you wish) somewhere meaningful, <br/>something like  "&#126;/.atom/" or "&#126;/.atom/packages/emmet/" etc..<br/>
  go to the Atom > Settings > packages > emmet > settings > Extension path <br/>
  set the path corresponding to the location of your Atom-emmet-extend-configuration-for-bem folder <br/>
  Relaunch atom.

## II) A less confusing syntax for the bem filter
  B : block <br />
  E : element<br />
  M : modifier<br />
  bem filter Syntax used in this config : B_E--M&nbsp;&nbsp;/&nbsp;&nbsp;B__E--M <br />
  <br />
  (Emmet default bem filter syntax is : B-E_M&nbsp;&nbsp;/&nbsp;&nbsp;B--E_M)

### II.1) Same examples as in emmet docs (web) with the new syntax
<pre>
  <code>
    .B--M
    &lt;div class="B B--M"&gt;&lt;/div&gt;

    .B--M1.--M2
    &lt;div class="B B--M1 B--M2"&gt;&lt;/div&gt;

    .B>.--M
    &lt;div class="B"&gt;
      &lt;div class="B B--M"&gt;&lt;/div&gt;
    &lt;/div&gt;

    .B1>.B2--M1>._E1+.__E2--M2
    &lt;div class="B1"&gt;
      &lt;div class="B2 B2--M1"&gt;
        &lt;div class="B2__E1"&gt;&lt;/div&gt;
        &lt;div class="B1__E2 B1__E2--M2"&gt;&lt;/div&gt;
      &lt;/div&gt;
    &lt;/div&gt;
  </code>
</pre>

