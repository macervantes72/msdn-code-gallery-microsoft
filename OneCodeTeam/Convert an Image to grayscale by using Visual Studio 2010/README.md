# Convert an Image to grayscale by using Visual Studio 2010
## Requires
- Visual Studio 2010
## License
- Apache License, Version 2.0
## Technologies
- GDI+
- Windows
- Windows Desktop App Development
## Topics
- image color change
## Updated
- 03/22/2016
## Description

<hr>
<div><a href="http://blogs.msdn.com/b/onecode" style="margin-top:3px"><img src="http://bit.ly/onecodesampletopbanner" alt="">
</a></div>
<h1>Samples to convert a colored image to gray scale by Visual Studio 2010</h1>
<h2>Introduction</h2>
<p class="MsoNormal">The sample codes developed in .NET Framework 4.0 would convert a colored image to gray scale using ColorMatrix class.</p>
<h2>Running the Sample</h2>
<p class="MsoNormal">Step 1: Open the &quot;ColorToGrayScale.sln&quot; file using VS 2010 or above.
<br>
Step 2: Build the code by pressing &quot;Ctrl&#43; Shift&#43; B&quot; key combination. <br>
Step 3: Execute the code either by clicking the F5 button or Ctrl &#43; F5.</p>
<h2>Using the Code</h2>
<h3>Below is the code snippet to convert a colored image to gray scale.</h3>
<p class="MsoNormal" style="margin-bottom:.0001pt; line-height:normal; text-autospace:none">
<span class="SpellE"><span class="GramE"><strong>ConvertToGrayScaleImage</strong></span></span><span class="GramE"><strong>(</strong></span><strong>) function</strong><span style="font-size:9.5pt; font-family:Consolas">
</span></p>
<p class="MsoNormal" style="margin-bottom:.0001pt; text-indent:.5in; line-height:normal; text-autospace:none">
<span style="font-size:9.5pt; font-family:Consolas; color:gray"><span>&nbsp;</span>///</span><span style="font-size:9.5pt; font-family:Consolas; color:green">
</span><span style="font-size:9.5pt; font-family:Consolas; color:gray">&lt;summary&gt;</span><span style="font-size:9.5pt; font-family:Consolas">
</span></p>
<p class="MsoNormal" style="margin-bottom:.0001pt; line-height:normal; text-autospace:none">
<span style="font-size:9.5pt; font-family:Consolas"><span>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
</span><span style="color:gray">///</span><span style="color:green"> This function converts a colored image to gray scale.</span>
</span></p>
<p class="MsoNormal" style="margin-bottom:.0001pt; line-height:normal; text-autospace:none">
<span style="font-size:9.5pt; font-family:Consolas"><span>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
</span><span style="color:gray">///</span><span style="color:green"> </span><span style="color:gray">&lt;/summary&gt;</span>
</span></p>
<p class="MsoNormal" style="margin-bottom:.0001pt; line-height:normal; text-autospace:none">
<span style="font-size:9.5pt; font-family:Consolas"><span>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
</span><span style="color:gray">///</span><span style="color:green"> </span><span style="color:gray">&lt;<span class="SpellE">param</span> name=&quot;<span class="SpellE">originalBitmap</span>&quot;&gt;</span>
</span></p>
<p class="MsoNormal" style="margin-bottom:.0001pt; line-height:normal; text-autospace:none">
<span style="font-size:9.5pt; font-family:Consolas"><span>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
</span><span style="color:gray">///</span><span style="color:green"> Bitmap handle to the source colored image.</span>
</span></p>
<p class="MsoNormal" style="margin-bottom:.0001pt; line-height:normal; text-autospace:none">
<span style="font-size:9.5pt; font-family:Consolas"><span>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
</span><span style="color:gray">///</span><span style="color:green"> </span><span style="color:gray">&lt;/<span class="SpellE">param</span>&gt;</span>
</span></p>
<p class="MsoNormal" style="margin-bottom:.0001pt; line-height:normal; text-autospace:none">
<span style="font-size:9.5pt; font-family:Consolas"><span>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
</span><span style="color:gray">///</span><span style="color:green"> </span><span style="color:gray">&lt;returns&gt;</span>
</span></p>
<p class="MsoNormal" style="margin-bottom:.0001pt; line-height:normal; text-autospace:none">
<span style="font-size:9.5pt; font-family:Consolas"><span>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
</span><span style="color:gray">///</span><span style="color:green"> Bitmap handle of the converted gray scale image.</span>
</span></p>
<p class="MsoNormal" style="margin-bottom:.0001pt; line-height:normal; text-autospace:none">
<span style="font-size:9.5pt; font-family:Consolas"><span>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
</span><span style="color:gray">///</span><span style="color:green"> </span><span style="color:gray">&lt;/returns&gt;</span>
</span></p>
<p class="MsoNormal" style="margin-bottom:.0001pt; line-height:normal; text-autospace:none">
<span style="font-size:9.5pt; font-family:Consolas">&nbsp;</span></p>
<p class="MsoNormal" style="margin-bottom:.0001pt; line-height:normal; text-autospace:none">
<span style="font-size:9.5pt; font-family:Consolas"><span>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
</span><span style="color:blue">private</span> <span style="color:blue">static</span>
<span style="color:#2b91af">Bitmap</span> <span class="SpellE"><span class="GramE">ConvertToGrayScaleImage</span></span><span class="GramE">(</span><span style="color:#2b91af">Bitmap</span>
<span class="SpellE">originalBitmap</span>) </span></p>
<p class="MsoNormal" style="margin-bottom:.0001pt; line-height:normal; text-autospace:none">
<span style="font-size:9.5pt; font-family:Consolas"><span>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
</span>{ </span></p>
<p class="MsoNormal" style="margin-bottom:.0001pt; line-height:normal; text-autospace:none">
<span style="font-size:9.5pt; font-family:Consolas"><span>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
</span><span style="color:green">// A blank bitmap is created having same size as original bitmap image.</span>
</span></p>
<p class="MsoNormal" style="margin-bottom:.0001pt; line-height:normal; text-autospace:none">
<span style="font-size:9.5pt; font-family:Consolas"><span>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
</span><span style="color:#2b91af">Bitmap</span> <span class="SpellE">GrayScaleBitmap</span> =
<span style="color:blue">new</span> <span class="GramE"><span style="color:#2b91af">Bitmap</span>(</span><span class="SpellE">originalBitmap.Width</span>,
<span class="SpellE">originalBitmap.Height</span>); </span></p>
<p class="MsoNormal" style="margin-bottom:.0001pt; line-height:normal; text-autospace:none">
<span style="font-size:9.5pt; font-family:Consolas">&nbsp;</span></p>
<p class="MsoNormal" style="margin-bottom:.0001pt; line-height:normal; text-autospace:none">
<span style="font-size:9.5pt; font-family:Consolas"><span>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
</span><span style="color:green">// Initializing a graphics object from the new image bitmap.</span>
</span></p>
<p class="MsoNormal" style="margin-bottom:.0001pt; line-height:normal; text-autospace:none">
<span style="font-size:9.5pt; font-family:Consolas"><span>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
</span><span style="color:#2b91af">Graphics</span> <span class="SpellE">graphics</span> =
<span class="SpellE"><span style="color:#2b91af">Graphics</span>.FromImage</span>(<span class="SpellE">GrayScaleBitmap</span>);
</span></p>
<p class="MsoNormal" style="margin-bottom:.0001pt; line-height:normal; text-autospace:none">
<span style="font-size:9.5pt; font-family:Consolas">&nbsp;</span></p>
<p class="MsoNormal" style="margin-bottom:.0001pt; line-height:normal; text-autospace:none">
<span style="font-size:9.5pt; font-family:Consolas"><span>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
</span><span style="color:green">// Creating the Grayscale ColorMatrix whose values are determined by</span>
</span></p>
<p class="MsoNormal" style="margin-bottom:.0001pt; line-height:normal; text-autospace:none">
<span style="font-size:9.5pt; font-family:Consolas"><span>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
</span><span style="color:green">// calculating the luminosity of a color, which is a weighted average of the</span>
</span></p>
<p class="MsoNormal" style="margin-bottom:.0001pt; line-height:normal; text-autospace:none">
<span style="font-size:9.5pt; font-family:Consolas"><span>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
</span><span style="color:green">// RGB color components. The average is weighted according to the sensitivity</span>
</span></p>
<p class="MsoNormal" style="margin-bottom:.0001pt; line-height:normal; text-autospace:none">
<span style="font-size:9.5pt; font-family:Consolas"><span>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
</span><span style="color:green">// of the human eye to each color component. The weights used here are as</span>
</span></p>
<p class="MsoNormal" style="margin-bottom:.0001pt; line-height:normal; text-autospace:none">
<span style="font-size:9.5pt; font-family:Consolas"><span>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
</span><span style="color:green">// given by the NTSC (North America Television Standards Committee)</span>
</span></p>
<p class="MsoNormal" style="margin-bottom:.0001pt; line-height:normal; text-autospace:none">
<span style="font-size:9.5pt; font-family:Consolas"><span>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
</span><span style="color:green">// and are widely accepted.</span> </span></p>
<p class="MsoNormal" style="margin-bottom:.0001pt; line-height:normal; text-autospace:none">
<span style="font-size:9.5pt; font-family:Consolas"><span>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
</span><span style="color:#2b91af">ColorMatrix</span> <span class="SpellE">colorMatrix</span> =
<span style="color:blue">new</span> <span class="GramE"><span style="color:#2b91af">ColorMatrix</span>(</span><span style="color:blue">new</span>
<span style="color:blue">float</span>[][] </span></p>
<p class="MsoNormal" style="margin-bottom:.0001pt; line-height:normal; text-autospace:none">
<span style="font-size:9.5pt; font-family:Consolas"><span>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
</span>{ </span></p>
<p class="MsoNormal" style="margin-bottom:.0001pt; line-height:normal; text-autospace:none">
<span style="font-size:9.5pt; font-family:Consolas"><span>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
</span><span style="color:blue">new</span> <span class="GramE"><span style="color:blue">float</span>[</span>] { 0.299f, 0.299f, 0.299f, 0, 0 },
</span></p>
<p class="MsoNormal" style="margin-bottom:.0001pt; line-height:normal; text-autospace:none">
<span style="font-size:9.5pt; font-family:Consolas"><span>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
</span><span style="color:blue">new</span> <span class="GramE"><span style="color:blue">float</span>[</span>] { 0.587f, 0.587f, 0.587f, 0, 0 },
</span></p>
<p class="MsoNormal" style="margin-bottom:.0001pt; line-height:normal; text-autospace:none">
<span style="font-size:9.5pt; font-family:Consolas"><span>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
</span><span style="color:blue">new</span> <span class="GramE"><span style="color:blue">float</span>[</span>] { 0.114f, 0.114f, 0.114f, 0, 0 },
</span></p>
<p class="MsoNormal" style="margin-bottom:.0001pt; line-height:normal; text-autospace:none">
<span style="font-size:9.5pt; font-family:Consolas"><span>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
</span><span style="color:blue">new</span> <span class="GramE"><span style="color:blue">float</span>[</span>] { 0,<span>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
</span>0,<span>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; </span>0,<span>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
</span>1, 0 }, </span></p>
<p class="MsoNormal" style="margin-bottom:.0001pt; line-height:normal; text-autospace:none">
<span style="font-size:9.5pt; font-family:Consolas"><span>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
</span><span style="color:blue">new</span> <span class="GramE"><span style="color:blue">float</span>[</span>] { 0,<span>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
</span>0,<span>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; </span>0,<span>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
</span>0, 1 } </span></p>
<p class="MsoNormal" style="margin-bottom:.0001pt; line-height:normal; text-autospace:none">
<span style="font-size:9.5pt; font-family:Consolas"><span>&nbsp;&nbsp;&nbsp;&nbsp;
</span><span>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</span>}); </span></p>
<p class="MsoNormal" style="margin-bottom:.0001pt; line-height:normal; text-autospace:none">
<span style="font-size:9.5pt; font-family:Consolas">&nbsp;</span></p>
<p class="MsoNormal" style="margin-bottom:.0001pt; line-height:normal; text-autospace:none">
<span style="font-size:9.5pt; font-family:Consolas"><span>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
</span><span style="color:green">// Creating image attributes.</span> </span></p>
<p class="MsoNormal" style="margin-bottom:.0001pt; line-height:normal; text-autospace:none">
<span style="font-size:9.5pt; font-family:Consolas"><span>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
</span><span class="SpellE"><span style="color:#2b91af">ImageAttributes</span></span> attributes =
<span style="color:blue">new</span> <span class="SpellE"><span class="GramE"><span style="color:#2b91af">ImageAttributes</span></span></span><span class="GramE">(</span>);
</span></p>
<p class="MsoNormal" style="margin-bottom:.0001pt; line-height:normal; text-autospace:none">
<span style="font-size:9.5pt; font-family:Consolas">&nbsp;</span></p>
<p class="MsoNormal" style="margin-bottom:.0001pt; line-height:normal; text-autospace:none">
<span style="font-size:9.5pt; font-family:Consolas"><span>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
</span><span style="color:green">// Setting the color matrix attribute.</span> </span>
</p>
<p class="MsoNormal" style="margin-bottom:.0001pt; line-height:normal; text-autospace:none">
<span style="font-size:9.5pt; font-family:Consolas"><span>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
</span><span class="SpellE"><span class="GramE">attributes.SetColorMatrix</span></span>(<span class="SpellE">colorMatrix</span>);
</span></p>
<p class="MsoNormal" style="margin-bottom:.0001pt; line-height:normal; text-autospace:none">
<span style="font-size:9.5pt; font-family:Consolas">&nbsp;</span></p>
<p class="MsoNormal" style="margin-bottom:.0001pt; line-height:normal; text-autospace:none">
<span style="font-size:9.5pt; font-family:Consolas"><span>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
</span><span style="color:green">// Drawing the original bitmap image on the new bitmap image using the</span>
</span></p>
<p class="MsoNormal" style="margin-bottom:.0001pt; line-height:normal; text-autospace:none">
<span style="font-size:9.5pt; font-family:Consolas"><span>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
</span><span style="color:green">// Grayscale color matrix.</span> </span></p>
<p class="MsoNormal" style="margin-bottom:.0001pt; line-height:normal; text-autospace:none">
<span style="font-size:9.5pt; font-family:Consolas"><span>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
</span><span class="SpellE"><span class="GramE">graphics.DrawImage</span></span>(<span class="SpellE">originalBitmap</span>,
<span style="color:blue">new</span> <span style="color:#2b91af">Rectangle</span>(0, 0,
<span class="SpellE">originalBitmap.Width</span>, </span></p>
<p class="MsoNormal" style="margin-bottom:.0001pt; line-height:normal; text-autospace:none">
<span style="font-size:9.5pt; font-family:Consolas"><span>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
</span><span class="SpellE">originalBitmap.Height</span>), 0, 0, <span class="SpellE">
originalBitmap.Width</span>, </span></p>
<p class="MsoNormal" style="margin-bottom:.0001pt; line-height:normal; text-autospace:none">
<span style="font-size:9.5pt; font-family:Consolas"><span>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
</span><span class="SpellE">originalBitmap.Height</span>, <span class="SpellE">
<span style="color:#2b91af">GraphicsUnit</span>.Pixel</span>, attributes); </span>
</p>
<p class="MsoNormal" style="margin-bottom:.0001pt; line-height:normal; text-autospace:none">
<span style="font-size:9.5pt; font-family:Consolas">&nbsp;</span></p>
<p class="MsoNormal" style="margin-bottom:.0001pt; line-height:normal; text-autospace:none">
<span style="font-size:9.5pt; font-family:Consolas"><span>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
</span><span style="color:green">// Disposing the Graphics object.</span> </span>
</p>
<p class="MsoNormal" style="margin-bottom:.0001pt; line-height:normal; text-autospace:none">
<span style="font-size:9.5pt; font-family:Consolas"><span>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
</span><span class="SpellE"><span class="GramE">graphics.Dispose</span></span>();
</span></p>
<p class="MsoNormal" style="margin-bottom:.0001pt; line-height:normal; text-autospace:none">
<span style="font-size:9.5pt; font-family:Consolas"><span>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
</span><span style="color:blue">return</span> <span class="SpellE">GrayScaleBitmap</span>;
</span></p>
<p class="MsoNormal" style="margin-bottom:.0001pt; line-height:normal; text-autospace:none">
<span style="font-size:9.5pt; font-family:Consolas"><span>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
</span>} </span></p>
<p class="MsoNormal" style="margin-bottom:.0001pt; text-indent:.5in; line-height:normal; text-autospace:none">
<span style="font-size:9.5pt; font-family:Consolas">&nbsp;</span></p>
<h3>Gray scale color matrix.</h3>
<p class="MsoNormal" style="margin-bottom:.0001pt; line-height:normal; text-autospace:none">
<span style="font-size:9.5pt; font-family:Consolas; color:green"><span>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
</span>// Grayscale ColorMatrix whose values are determined by calculating</span><span style="font-size:9.5pt; font-family:Consolas">
</span></p>
<p class="MsoNormal" style="margin-bottom:.0001pt; line-height:normal; text-autospace:none">
<span style="font-size:9.5pt; font-family:Consolas"><span>&nbsp;</span><span>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
</span><span style="color:green">// the luminosity of a color, which is a weighted average of the RGB</span>
</span></p>
<p class="MsoNormal" style="margin-bottom:.0001pt; line-height:normal; text-autospace:none">
<span style="font-size:9.5pt; font-family:Consolas"><span>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
</span><span style="color:green">// color components. The average is weighted according to the sensitivity</span>
</span></p>
<p class="MsoNormal" style="margin-bottom:.0001pt; line-height:normal; text-autospace:none">
<span style="font-size:9.5pt; font-family:Consolas"><span>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
</span><span style="color:green">// of the human eye to each color component. The weights used here are as</span>
</span></p>
<p class="MsoNormal" style="margin-bottom:.0001pt; line-height:normal; text-autospace:none">
<span style="font-size:9.5pt; font-family:Consolas"><span>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
</span><span style="color:green">// given by the NTSC (North America Television Standards Committee)</span>
</span></p>
<p class="MsoNormal" style="margin-bottom:.0001pt; line-height:normal; text-autospace:none">
<span style="font-size:9.5pt; font-family:Consolas"><span>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
</span><span style="color:green">// and are widely accepted.</span> </span></p>
<p class="MsoNormal" style="margin-bottom:.0001pt; line-height:normal; text-autospace:none">
<span style="font-size:9.5pt; font-family:Consolas"><span>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
</span><span style="color:#2b91af">ColorMatrix</span> <span class="SpellE">colorMatrix</span> =
<span style="color:blue">new</span> <span class="GramE"><span style="color:#2b91af">ColorMatrix</span>(</span><span style="color:blue">new</span>
<span style="color:blue">float</span>[][] </span></p>
<p class="MsoNormal" style="margin-bottom:.0001pt; line-height:normal; text-autospace:none">
<span style="font-size:9.5pt; font-family:Consolas"><span>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
</span>{ </span></p>
<p class="MsoNormal" style="margin-bottom:.0001pt; line-height:normal; text-autospace:none">
<span style="font-size:9.5pt; font-family:Consolas"><span>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
</span><span style="color:blue">new</span> <span class="GramE"><span style="color:blue">float</span>[</span>] { 0.299f, 0.299f, 0.299f, 0, 0 },
</span></p>
<p class="MsoNormal" style="margin-bottom:.0001pt; line-height:normal; text-autospace:none">
<span style="font-size:9.5pt; font-family:Consolas"><span>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
</span><span style="color:blue">new</span> <span class="GramE"><span style="color:blue">float</span>[</span>] { 0.587f, 0.587f, 0.587f, 0, 0 },
</span></p>
<p class="MsoNormal" style="margin-bottom:.0001pt; line-height:normal; text-autospace:none">
<span style="font-size:9.5pt; font-family:Consolas"><span>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
</span><span style="color:blue">new</span> <span class="GramE"><span style="color:blue">float</span>[</span>] { 0.114f, 0.114f, 0.114f, 0, 0 },
</span></p>
<p class="MsoNormal" style="margin-bottom:.0001pt; line-height:normal; text-autospace:none">
<span style="font-size:9.5pt; font-family:Consolas"><span>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
</span><span style="color:blue">new</span> <span class="GramE"><span style="color:blue">float</span>[</span>] { 0,<span>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
</span>0,<span>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; </span>0,<span>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
</span>1, 0 }, </span></p>
<p class="MsoNormal" style="margin-bottom:.0001pt; line-height:normal; text-autospace:none">
<span style="font-size:9.5pt; font-family:Consolas"><span>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
</span><span style="color:blue">new</span> <span class="GramE"><span style="color:blue">float</span>[</span>] { 0,<span>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
</span>0,<span>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; </span>0,<span>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
</span>0, 1 } </span></p>
<p class="MsoNormal" style="margin-bottom:.0001pt; line-height:normal; text-autospace:none">
<span style="font-size:9.5pt; font-family:Consolas"><span>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
</span>}); </span></p>
<p class="MsoNormal" style="margin-bottom:.0001pt; line-height:normal; text-autospace:none">
<span style="font-size:10.0pt; font-family:&quot;Courier New&quot;">&nbsp;</span></p>
<p class="MsoListParagraphCxSpFirst" style="margin-left:0in">&nbsp;</p>
<p class="MsoListParagraphCxSpMiddle" style="margin-left:0in">&nbsp;</p>
<p class="MsoListParagraphCxSpMiddle" style="text-indent:-.25in; line-height:150%">
<span style="font-family:Symbol"><span>&bull;<span style="font:7.0pt &quot;Times New Roman&quot;">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
</span></span></span>Click on <strong>Choose File&hellip; </strong>menu to select the colored source image.<strong>
</strong></p>
<p class="MsoListParagraphCxSpMiddle" style="text-indent:-.25in; line-height:150%">
<span style="font-family:Symbol"><span>&bull;<span style="font:7.0pt &quot;Times New Roman&quot;">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
</span></span></span>Click on <strong>Convert</strong> menu to perform colored to gray scale image conversion.<strong>
</strong></p>
<p class="MsoListParagraphCxSpMiddle" style="text-indent:-.25in; line-height:150%">
<span style="font-family:Symbol"><span>&bull;<span style="font:7.0pt &quot;Times New Roman&quot;">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
</span></span></span>Click on <strong>Save Output </strong>menu to save the converted gray scale image output to a local directory.<strong>
</strong></p>
<p class="MsoListParagraphCxSpMiddle" style="text-indent:-.25in; line-height:150%">
<span style="font-family:Symbol"><span>&bull;<span style="font:7.0pt &quot;Times New Roman&quot;">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
</span></span></span>Click on <strong>Reset</strong> menu to clear out source and converted image spaces.
<strong>&nbsp;</strong></p>
<p class="MsoListParagraphCxSpLast"><strong>&nbsp;</strong></p>
<p style="line-height:0.6pt; color:white">Microsoft All-In-One Code Framework is a free, centralized code sample library driven by developers' real-world pains and needs. The goal is to provide customer-driven code samples for all Microsoft development technologies,
 and reduce developers' efforts in solving typical programming tasks. Our team listens to developers&rsquo; pains in the MSDN forums, social media and various DEV communities. We write code samples based on developers&rsquo; frequently asked programming tasks,
 and allow developers to download them with a short sample publishing cycle. Additionally, we offer a free code sample request service. It is a proactive way for our developer community to obtain code samples directly from Microsoft.</p>
<hr>
<div><a href="http://go.microsoft.com/?linkid=9759640" style="margin-top:3px"><img src="http://bit.ly/onecodelogo" alt="">
</a></div>
