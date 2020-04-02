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
Here it is.  Recreated it 
    
    draw fullcircle scaled 2cm shifted (-0.5cm,0cm);
    draw fullcircle scaled 2cm shifted (0.5cm,0cm);
    draw fullcircle scaled 2cm shifted (0cm,-1cm);
    label bot ( btex $3$ etex, (0,0) );
    label bot ( btex $7$ etex, (0,-1.2cm) );
    label top ( btex $2$ etex, (0,0) );
    label top ( btex $8$ etex, (-0.9cm,0) );
    label top ( btex $15$ etex, (0.8cm,0) );
    label bot ( btex $9$ etex, (-0.6cm,-0.4cm) );
    label bot ( btex $6$ etex, 
(0.6cm,-0.4cm) );
    label bot ( btex $10$ etex, (-1.4cm,-1.95cm) );
    label ulft ( btex $\mbox{Soccer}$ etex, (-0.9cm,1.1cm) );
    label urt ( btex $\mbox{Basketball}$ 
