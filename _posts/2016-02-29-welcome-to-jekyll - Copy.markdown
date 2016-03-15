---
layout: post
title:  "Welcome to Jekyll!"
date:   2016-02-29 22:59:27 +0100
categories: jekyll update
---
You’ll find this post in your `_posts` directory. Go ahead and edit it and re-build the site to see your changes. You can rebuild the site in many different ways, but the most common way is to run `jekyll serve`, which launches a web server and auto-regenerates your site when a file is updated.

To add new posts, simply add a file in the `_posts` directory that follows the convention `YYYY-MM-DD-name-of-post.ext` and includes the necessary front matter. Take a look at the source for this post to get an idea about how it works.

Jekyll also offers powerful support for code snippets:

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
