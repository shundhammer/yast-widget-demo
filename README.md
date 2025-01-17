# YaST Widget Demo

This repository is a demo for most of the widgets provided by the YaST user
interface.

The main purpose is to provide an easily accessible sample of the widgets for
editing Qt widget style sheets.



## Building and Installing

- Make sure the `yast-rake` Ruby gem for your ruby version is installed
  (`ruby2.7-rubygem-yast-rake` at the time of this writing):

      sudo zypper install "ruby*-rubygem-yast-rake"

- Install:

      sudo rake install



## How to Run

- Graphical (Qt) version:

      yast2 widget_demo
      
  or
  
      yast2 widget_demo_no_wizard_steps

- Text-based (NCurses) version:

      yast widget_demo


## Permissions

No root privileges are required for this YaST module.


## Using a Different Widget Style Sheet

The Qt UI uses one of the `.qss` widget style sheets in
`/usr/share/YaST2/theme/current/wizard`. The default is `style.qss`.

Set the Y2STYLE environment variable to use a different style sheet:

    Y2STYLE=installation.qss yast2 widget_demo

Once the demo is running, you can use the style sheet editor with
`Ctrl-Shift-Alt-S`.


## Screenshot

![widget-demo-tw-01](https://user-images.githubusercontent.com/11538225/119511524-cbea8d80-bd72-11eb-9c92-81d63eff0085.png)


More screenshots at
https://github.com/yast/yast-widget-demo/issues/2


## Reference

- [Qt widget style sheet reference](https://doc.qt.io/qt-5/stylesheet-reference.html)

- [YaST QSS for SLE](https://github.com/yast/yast-theme/blob/master/theme/SLE/wizard/installation.qss)

- [YaST QSS for openSUSE Leap 15.3](https://github.com/openSUSE/branding/blob/leap-15.3/yast/installation.qss)

  (switch to another branch in that repository for the theme of a different
  openSUSE distribution)

- [YaST UI reference documentation](https://doc.opensuse.org/projects/YaST/openSUSE11.3/tdg/Book-UIReference.html)

- [YaST UI examples](https://github.com/yast/yast-ycp-ui-bindings/tree/master/examples)

- [YaST documentation](https://yastgithubio.readthedocs.io/en/latest/) at readthedocs.io
