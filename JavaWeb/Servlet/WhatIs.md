# Servlet
```md
Servlet是Java平台上的CGI技术
	它在服务器端运行，用以动态生成Web页面
	与传统的CGI和许多其他类似CGI的技术相比，Java Servlet具有更高的效率，它依靠线程的方式来支持并发访问。
```
```md
背景
	Servlet最初是在1995年由James Gosling 提出的，因为使用该技术需要复杂的Web服务器支持，所以当时并没有得到重视，也就放弃了。
	后来随着Web应用复杂度的提升，并要求提供更高的并发处理能力，Servlet被重新捡起，并在Java平台上得到实现，现在提起Servlet，指的都是Java Servlet。
```
```md
优势
	对每个请求都是单独启动一个线程，而不是进程
		大幅度地降低了系统里的进程数量，提高了系统的并发处理能力。
	因为Java Servlet是运行在虚拟机之上的，也就解决了跨平台问题
```
* 与WebServer
```md
必须运行在Web服务器当中，与Web服务器之间属于分工和互补关系。
确切的说，在实际运行的时候Java Servlet与Web服务器会融为一体，
如同一个程序一样运行在同一个Java虚拟机（JVM）当中。
```
* 与Servlet 容器
```md
Servlet 没有 main 方法，不能够独立的运行，它的运行需要容器的支持，Tomcat 是最常用的 JSP/Servlet 容器。
Servlet 运行在 Servlet 容器中，并由容器管理从创建到销毁的整个过程。
它们是彼此依存的，但是又相互独立发展，这一切都是为了适应工业化生产的结果。
从技术角度来说是为了解耦，通过标准化接口来相互协作。
```