---
layout: post
title:  "To jest pierwszy post!"
date:   2016-02-27 22:59:27 +0100
categories: jekyll update
tags: [java, gameart]
---
Lorem ipsum dolor sit amet eros. Nullam semper nisl, semper magna tincidunt wisi adipiscing elit. Proin non eros pellentesque leo. Ut tempus enim ac lacus. Maecenas mi quam ipsum, rutrum posuere a, sodales sapien pede eget orci luctus quam in turpis in ligula ut lacus lacus tincidunt turpis egestas. Mauris vitae ante. Integer nibh sit amet, consectetuer ut, faucibus quis, dui. Aliquam interdum pellentesque at, egestas velit. 

Donec enim eu nibh. Maecenas mi eget imperdiet faucibus ipsum dolor nulla, accumsan nisl sapien auctor euismod. Integer mi at consectetuer tincidunt est congue et, posuere sed, sodales nibh nulla, accumsan sed, venenatis consequat. Morbi congue arcu. Aenean quis blandit eros, sagittis malesuada. Ut blandit, dui auctor ligula. Nulla consectetuer, augue eu sapien. Vestibulum quam. Vestibulum ante sodales pretium convallis. Donec pharetra lobortis augue nec massa. 

Duis mauris nibh consectetuer sagittis lorem. In hac habitasse platea dictumst. Sed elementum, sapien sed massa in dolor sed interdum mi mauris, consectetuer adipiscing metus. Proin posuere. In tempus. Pellentesque eu nulla. Curabitur ultrices posuere ante sit amet lacus. Nulla augue quis faucibus et, faucibus orci et.

{% highlight java %}
package atmos.tool2d;

import com.badlogic.gdx.ApplicationListener;
import com.badlogic.gdx.Gdx;
import com.badlogic.gdx.backends.lwjgl.LwjglApplication;
import com.badlogic.gdx.backends.lwjgl.LwjglApplicationConfiguration;
import com.badlogic.gdx.graphics.OrthographicCamera;
import com.badlogic.gdx.graphics.Pixmap.Format;
import com.badlogic.gdx.graphics.Texture;
import com.badlogic.gdx.graphics.g2d.SpriteBatch;
import com.badlogic.gdx.graphics.glutils.ShaderProgram;

/**
 * A port of ShaderLesson1 from lwjgl-basics to LibGDX:
 * https://github.com/mattdesl/lwjgl-basics/wiki/ShaderLesson1
 * 
 * @author davedes
 */
public class ShaderLesson1 implements ApplicationListener {
	
	//Minor differences: 
		//LibGDX Position attribute is a vec4
		//u_projView is called u_projTrans
		//we need to set ShaderProgram.pedantic to false 
		//LibGDX uses lower-left as origin (0, 0)
	
	public static void main(String[] args) {
		LwjglApplicationConfiguration cfg = 
		new LwjglApplicationConfiguration();
		
		cfg.title = "Shader Lesson 1";
		cfg.useGL20 = true;
		cfg.width = 640;
		cfg.height = 480;
		cfg.resizable = false;

		new LwjglApplication(new ShaderLesson1(), cfg);
	}

{% endhighlight %}

Check out the [Jekyll docs][jekyll-docs] for more info on how to get the most out of Jekyll. File all bugs/feature requests at [Jekyll’s GitHub repo][jekyll-gh]. If you have questions, you can ask them on [Jekyll Talk][jekyll-talk].



[jekyll-docs]: http://jekyllrb.com/docs/home
[jekyll-gh]:   https://github.com/jekyll/jekyll
[jekyll-talk]: https://talk.jekyllrb.com/
