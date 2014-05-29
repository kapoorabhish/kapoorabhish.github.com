---
layout: post
title: "how we test browsers!!"
date: 2013-06-04 18:07
comments: true
categories: 
---
by CNET


 The Web browser is the most-used kind of software in the world, having become the de facto way that people access the Internet. Today, virtually all computing tasks can be completed in the browser.

Testing browsers can veer from incredibly complex to shockingly simple, depending on what you're looking for and why. At CNET, we prefer a holistic approach to browser benchmarking, looking at a combination of tests that benchmark general browser behavior, as well as several "real-world" tests that look at browser performance in common scenarios. 


<h3>How we test desktop browsers</h3>

We run each of the following three times, and restart the computer before each test, so that the browser is starting "cold." We also wait 30 seconds after booting the browser to ensure that any background processes have been completed. Then we average the three tests.


<h3>  Performance benchmarks</h3>
The <a href="http://acid3.acidtests.org/">Acid3</a> test from the <a href="http://www.webstandards.org/">Web Standards Project</a> checks browser compliance with accepted standards. Slightly outdated since it doesn't look at HTML5, which has now been finalized, it remains a good way to establish a baseline. Browsers that don't hit 100 out of 100 on the Acid3 are behind the times in a fundamental, crucial way.

<a href=https://developers.google.com/octane/  target=_blank" >Google Octane</a>, the successor to Google's <a href=http://v8.googlecode.com/svn/data/benchmarks/v7/run.html target=_blank>  V8 benchmark test</a>, looks at JavaScript performance by testing such areas as code optimization, encryption and decryption, emulation, and array manipulation, and assigning each subtest a number. The higher the final score, the better.

<a href=http://krakenbenchmark.mozilla.org/ target=_blank>Mozilla Kraken</a> is another JavaScript performance test, which looks specifically at rendering times for audio, imaging, AI, JSON, and encryption. A smaller number is better for the final score.

The <a href=http://html5test.com/ target=_blank>HTML5 Test</a> assigns points for each HTML5 feature that the browser supports, out of a total of 500. This is a rough way to gauge how future-forward the browser is.

<a href=https://github.com/facebook/jsgamebench/ target=_blank>JSGameBench</a>, GUImark3 (<a href=http://www.craftymind.com/factory/guimark2/HTML5GamingTest.html target=_blank>gaming test</a>, <a href=http://www.craftymind.com/factory/guimark2/HTML5TextTest.html target=_blank >text test</a>), and <a href=http://ie.microsoft.com/testdrive/views/sitemap target=_blank >Microsoft FishIE Tank </a>look at HTML5 Canvas performance in several different game-like environments. Canvas is an important part of HTML5 to test because it creates all the nifty 2D images and shapes that can move across your screen. 

 Each of these three tests uses a different standard. FishIE Tank, for example, lets the tester set the number of fish on the screen. The test will then show you in how many frames per second they can be rendered.

Microsoft Chalkboard runs a series of timed tests on HTML5 panning, zooming, and scaling. Faster is better.

Facebook Ringmark checks HTML5 feature support, geared for the needs of the mobile browser. Nevertheless, it works well on desktops and provides a good and rare point of comparison between desktop and mobile. 
