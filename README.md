![](media/8c8866a288ed0453894f09791c729de6.png)

**Background**

When working with mobile applications, trying to place all your code on one form
can become cumbersome. So to overcome this you will need to create forms and
dock forms onto a main form permanently or temporarily. If you believed that FMX
form Docking is the same as VCL, then this blog will help you to make the new
implementation easier because the FMX method is a lot different from the VCL
method.

**IDE**

Tokyo 10.2 used, this should be backwards compatible to Post XE4 versions.

**Scope**

Dock different forms to a specific tab-item in the tab-control of a form and
free them when required.

**Requirements**

Standard FMX Library.

Difficulty level - Low.

**Method**

**How does it work?**

-   The Form to be ‘**Docked to’** must have a Tlayout or Tpanel or similar
    which becomes the Parent object to be docked to.

-   The Form to be ‘**Dockedfrom**’ must have a Tlayout or Tpanel or similar
    which becomes the Child of the Parent.

-   All the children ( Tedits, Tbuttons,Tlabels, etc) of the ‘**DockedFrom**’
    form become the children of the Parent and are added in the order in which
    they were created at design time.

So if you will be reusing the ‘**Dockedto**’ as the parent to add and remove
different forms,

>   a new step will need to be added else further docking will result in the
>   loaded form’s children being overlaid on each other resulting in an unusable
>   mess.

Read my blog to get the full information on how to impliment docking:-
[](https://bayeseanblog.com/blog/delphi-fmx-form-docking/17)

[Delphi-FMX-form-docking](media/f95a892a100ee0af7c77fdebee23cae3.png)


![](media/c9c865d333eecdd2804d8c67665d89ff.png)

![](media/4308e0bdfc554d5a42d87e2905135b0b.png)



Happy Coding
