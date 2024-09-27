---
title: "TinyGo Home"
---

{{< blocks/cover title="TinyGo - A Go Compiler For Small Places" image_anchor="top" height="full" color="primary" >}}

![TinyGo Logo](images/tinygo-logo.png)

<div class="mx-auto">
	<a class="btn btn-lg btn-primary mr-3 mb-4" href="{{< relref "/getting-started" >}}">
		Get Started <i class="fas fa-arrow-alt-circle-right ml-2"></i>
	</a>
	<a class="btn btn-lg btn-secondary mr-3 mb-4" href="https://github.com/tinygo-org/tinygo">
		See the code <i class="fab fa-github ml-2 "></i>
	</a>
	<p class="h2 mt-5">Go on embedded systems and WebAssembly</p>
</div>
{{< /blocks/cover >}}

{{% blocks/lead color="secondary" %}}
TinyGo brings the [Go programming language](https://golang.org) to embedded systems and to the modern web by creating a new compiler based on [LLVM](https://llvm.org/).

You can compile and run TinyGo programs on over 100 different microcontroller boards from maker boards such as the [BBC micro:bit](https://www.microbit.co.uk/) and the [Arduino Uno](https://store.arduino.cc/usa/arduino-uno-rev3/), to industrial processors from [Nordic Semiconductor](https://www.nordicsemi.com/) and [ST Microelectronics](https://www.st.com/). [Click here for the complete list](/docs/reference/microcontrollers)

TinyGo can also produce [WebAssembly (WASM)](https://webassembly.org/) code which is very compact in size. You can compile programs for web browsers, as well as for server and edge computing environments that support the [WebAssembly System Interface (WASI)](https://github.com/WebAssembly/WASI) family of interfaces.

Ready to get started? [Click here](getting-started).

{{% /blocks/lead %}}

{{% blocks/section color="primary-light" %}}
<link rel="stylesheet" href="playground/simulator.css">
<link rel="stylesheet" href="playground/simulator-bootstrap.css">
<script type="module" src="playground-home.js"></script>
<link rel="modulepreload" href="/playground/resources/editor.bundle.min.js"/>
<div class="col">
	<div class="container" id="playground">
		<h1 class="text-center">Try TinyGo</h1>
		<div class="row px-0">
			<div class="col col-auto">
				<div class="input-group mb-3">
					<span class="input-group-text">Example</span>
					<select class="form-select example_select" disabled>
						<option value="hello">Hello world</option>
						<option value="arduino" selected>Blinking LED (Arduino Uno)</option>
						<option value="circuitplay_express">RGB LEDs (Adafruit Circuit Playground Express)</option>
						<option value="gopher_badge">Display (Gopher Badge)</option>
					</select>
				</div>
			</div>
			<div class="col col-auto">
				<button class="btn btn-secondary playground-btn-flash mb-3" disabled>Download binary</button>
				<a href="/tour/" class="btn btn-link mb-3">Tour of TinyGo</a>
			</div>
		</div>
		<div class="playground-editor mb-3" tabindex="-1"></div>
		<div class="simulator">{{< readfile "/simulator/simulator.md" >}}</div>
	</div>
</div>
{{% /blocks/section %}}

{{< blocks/section color="primary" type="row" >}}
{{% blocks/feature icon="fa-lightbulb" title="TinyGo Playground" url="/play/" %}}
Try TinyGo online
{{% /blocks/feature %}}

{{% blocks/feature icon="fab fa-github" title="TinyGo on Github" url="https://github.com/tinygo-org/tinygo" %}}
See the code here
{{% /blocks/feature %}}


{{% blocks/feature icon="fab fa-mastodon" title="TinyGo on Mastodon" url="https://mastodon.social/@TinyGo" %}}
Join us on Mastodon
{{% /blocks/feature %}}

{{< /blocks/section >}}

