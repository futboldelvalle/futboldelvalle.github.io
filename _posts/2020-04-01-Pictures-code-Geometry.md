# Picture Code for Geometry

Use [http://www.tlhiv.org/mppreview/](http://www.tlhiv.org/mppreview/)
And cut paste code

30-60-90 Right Triangle

    pair A, B, C;
    A:=(0,0); B:=(0.5cm,0.8660cm); C:=(0.5cm,0);
    draw A--B--C--cycle;
    draw unitsquare scaled 0.125cm shifted (0.375cm,0);
    label.rt(btex $a\sqrt{3}$ etex, 1/2[B,C]);
    label.llft(btex $a$ etex, 1/2[A,C]);
    label.ulft(btex $2a$ etex, 1/2[A,B]);
    label.rt(btex $\mbox{30-60-90}$ etex, (-0.025cm,-0.5cm));

Output should look like
![Metapost Previewer](/images/Screenshot_20200401-212607.png)

45-45-90 Right Triangle

    pair A, B, C;
    A:=(0,0); B:=(1cm,1cm); C:=(1cm,0);
    draw A--B--C--cycle;
    draw unitsquare scaled 0.125cm shifted (0.875cm,0);
    label.lrt(btex $a$ etex, 1/2[B,C]);
    label.llft(btex $a$ etex, 1/2[A,C]);
    label.ulft(btex $a\sqrt{2}$ etex, 1/2[A,B]);
    label.rt(btex $\mbox{45-45-90}$ etex, (-0.025cm,-0.5cm));

You can create a spreadsheet using google sheets to create
Pythagorean triples.

![Screenshot 1](/images/Screenshot_20200401-205417.png)

![Screenshot 2](/images/Screenshot_20200401-210146.png)

I will upload code for Venn Diagram later.  Have it on laptop. Please be patient.

