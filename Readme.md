<html><head><meta http-equiv="Content-Type" content="text/html; charset=utf-8"/><title>React snippets extension</title><style>
/* cspell:disable-file */
/* webkit printing magic: print all background colors */
html {
	-webkit-print-color-adjust: exact;
}
* {
	box-sizing: border-box;
	-webkit-print-color-adjust: exact;
}

html,
body {
	margin: 0;
	padding: 0;
}
@media only screen {
	body {
		margin: 2em auto;
		max-width: 900px;
		color: rgb(55, 53, 47);
	}
}

body {
	line-height: 1.5;
	white-space: pre-wrap;
}

a,
a.visited {
	color: inherit;
	text-decoration: underline;
}

.pdf-relative-link-path {
	font-size: 80%;
	color: #444;
}

h1,
h2,
h3 {
	letter-spacing: -0.01em;
	line-height: 1.2;
	font-weight: 600;
	margin-bottom: 0;
}

.page-title {
	font-size: 2.5rem;
	font-weight: 700;
	margin-top: 0;
	margin-bottom: 0.75em;
}

h1 {
	font-size: 1.875rem;
	margin-top: 1.875rem;
}

h2 {
	font-size: 1.5rem;
	margin-top: 1.5rem;
}

h3 {
	font-size: 1.25rem;
	margin-top: 1.25rem;
}

.source {
	border: 1px solid #ddd;
	border-radius: 3px;
	padding: 1.5em;
	word-break: break-all;
}

.callout {
	border-radius: 3px;
	padding: 1rem;
}

figure {
	margin: 1.25em 0;
	page-break-inside: avoid;
}

figcaption {
	opacity: 0.5;
	font-size: 85%;
	margin-top: 0.5em;
}

mark {
	background-color: transparent;
}

.indented {
	padding-left: 1.5em;
}

hr {
	background: transparent;
	display: block;
	width: 100%;
	height: 1px;
	visibility: visible;
	border: none;
	border-bottom: 1px solid rgba(55, 53, 47, 0.09);
}

img {
	max-width: 100%;
}

@media only print {
	img {
		max-height: 100vh;
		object-fit: contain;
	}
}

@page {
	margin: 1in;
}

.collection-content {
	font-size: 0.875rem;
}

.column-list {
	display: flex;
	justify-content: space-between;
}

.column {
	padding: 0 1em;
}

.column:first-child {
	padding-left: 0;
}

.column:last-child {
	padding-right: 0;
}

.table_of_contents-item {
	display: block;
	font-size: 0.875rem;
	line-height: 1.3;
	padding: 0.125rem;
}

.table_of_contents-indent-1 {
	margin-left: 1.5rem;
}

.table_of_contents-indent-2 {
	margin-left: 3rem;
}

.table_of_contents-indent-3 {
	margin-left: 4.5rem;
}

.table_of_contents-link {
	text-decoration: none;
	opacity: 0.7;
	border-bottom: 1px solid rgba(55, 53, 47, 0.18);
}

table,
th,
td {
	border: 1px solid rgba(55, 53, 47, 0.09);
	border-collapse: collapse;
}

table {
	border-left: none;
	border-right: none;
}

th,
td {
	font-weight: normal;
	padding: 0.25em 0.5em;
	line-height: 1.5;
	min-height: 1.5em;
	text-align: left;
}

th {
	color: rgba(55, 53, 47, 0.6);
}

ol,
ul {
	margin: 0;
	margin-block-start: 0.6em;
	margin-block-end: 0.6em;
}

li > ol:first-child,
li > ul:first-child {
	margin-block-start: 0.6em;
}

ul > li {
	list-style: disc;
}

ul.to-do-list {
	text-indent: -1.7em;
}

ul.to-do-list > li {
	list-style: none;
}

.to-do-children-checked {
	text-decoration: line-through;
	opacity: 0.375;
}

ul.toggle > li {
	list-style: none;
}

ul {
	padding-inline-start: 1.7em;
}

ul > li {
	padding-left: 0.1em;
}

ol {
	padding-inline-start: 1.6em;
}

ol > li {
	padding-left: 0.2em;
}

.mono ol {
	padding-inline-start: 2em;
}

.mono ol > li {
	text-indent: -0.4em;
}

.toggle {
	padding-inline-start: 0em;
	list-style-type: none;
}

/* Indent toggle children */
.toggle > li > details {
	padding-left: 1.7em;
}

.toggle > li > details > summary {
	margin-left: -1.1em;
}

.selected-value {
	display: inline-block;
	padding: 0 0.5em;
	background: rgba(206, 205, 202, 0.5);
	border-radius: 3px;
	margin-right: 0.5em;
	margin-top: 0.3em;
	margin-bottom: 0.3em;
	white-space: nowrap;
}

.collection-title {
	display: inline-block;
	margin-right: 1em;
}

.simple-table {
	margin-top: 1em;
	font-size: 0.875rem;
	empty-cells: show;
}
.simple-table td {
	height: 29px;
	min-width: 120px;
}

.simple-table th {
	height: 29px;
	min-width: 120px;
}

.simple-table-header-color {
	background: rgb(247, 246, 243);
	color: black;
}
.simple-table-header {
	font-weight: 500;
}

time {
	opacity: 0.5;
}

.icon {
	display: inline-block;
	max-width: 1.2em;
	max-height: 1.2em;
	text-decoration: none;
	vertical-align: text-bottom;
	margin-right: 0.5em;
}

img.icon {
	border-radius: 3px;
}

.user-icon {
	width: 1.5em;
	height: 1.5em;
	border-radius: 100%;
	margin-right: 0.5rem;
}

.user-icon-inner {
	font-size: 0.8em;
}

.text-icon {
	border: 1px solid #000;
	text-align: center;
}

.page-cover-image {
	display: block;
	object-fit: cover;
	width: 100%;
	max-height: 30vh;
}

.page-header-icon {
	font-size: 3rem;
	margin-bottom: 1rem;
}

.page-header-icon-with-cover {
	margin-top: -0.72em;
	margin-left: 0.07em;
}

.page-header-icon img {
	border-radius: 3px;
}

.link-to-page {
	margin: 1em 0;
	padding: 0;
	border: none;
	font-weight: 500;
}

p > .user {
	opacity: 0.5;
}

td > .user,
td > time {
	white-space: nowrap;
}

input[type="checkbox"] {
	transform: scale(1.5);
	margin-right: 0.6em;
	vertical-align: middle;
}

p {
	margin-top: 0.5em;
	margin-bottom: 0.5em;
}

.image {
	border: none;
	margin: 1.5em 0;
	padding: 0;
	border-radius: 0;
	text-align: center;
}

.code,
code {
	background: rgba(135, 131, 120, 0.15);
	border-radius: 3px;
	padding: 0.2em 0.4em;
	border-radius: 3px;
	font-size: 85%;
	tab-size: 2;
}

code {
	color: #eb5757;
}

.code {
	padding: 1.5em 1em;
}

.code-wrap {
	white-space: pre-wrap;
	word-break: break-all;
}

.code > code {
	background: none;
	padding: 0;
	font-size: 100%;
	color: inherit;
}

blockquote {
	font-size: 1.25em;
	margin: 1em 0;
	padding-left: 1em;
	border-left: 3px solid rgb(55, 53, 47);
}

.bookmark {
	text-decoration: none;
	max-height: 8em;
	padding: 0;
	display: flex;
	width: 100%;
	align-items: stretch;
}

.bookmark-title {
	font-size: 0.85em;
	overflow: hidden;
	text-overflow: ellipsis;
	height: 1.75em;
	white-space: nowrap;
}

.bookmark-text {
	display: flex;
	flex-direction: column;
}

.bookmark-info {
	flex: 4 1 180px;
	padding: 12px 14px 14px;
	display: flex;
	flex-direction: column;
	justify-content: space-between;
}

.bookmark-image {
	width: 33%;
	flex: 1 1 180px;
	display: block;
	position: relative;
	object-fit: cover;
	border-radius: 1px;
}

.bookmark-description {
	color: rgba(55, 53, 47, 0.6);
	font-size: 0.75em;
	overflow: hidden;
	max-height: 4.5em;
	word-break: break-word;
}

.bookmark-href {
	font-size: 0.75em;
	margin-top: 0.25em;
}

.sans { font-family: ui-sans-serif, -apple-system, BlinkMacSystemFont, "Segoe UI", Helvetica, "Apple Color Emoji", Arial, sans-serif, "Segoe UI Emoji", "Segoe UI Symbol"; }
.code { font-family: "SFMono-Regular", Menlo, Consolas, "PT Mono", "Liberation Mono", Courier, monospace; }
.serif { font-family: Lyon-Text, Georgia, ui-serif, serif; }
.mono { font-family: iawriter-mono, Nitti, Menlo, Courier, monospace; }
.pdf .sans { font-family: Inter, ui-sans-serif, -apple-system, BlinkMacSystemFont, "Segoe UI", Helvetica, "Apple Color Emoji", Arial, sans-serif, "Segoe UI Emoji", "Segoe UI Symbol", 'Twemoji', 'Noto Color Emoji', 'Noto Sans CJK JP'; }
.pdf:lang(zh-CN) .sans { font-family: Inter, ui-sans-serif, -apple-system, BlinkMacSystemFont, "Segoe UI", Helvetica, "Apple Color Emoji", Arial, sans-serif, "Segoe UI Emoji", "Segoe UI Symbol", 'Twemoji', 'Noto Color Emoji', 'Noto Sans CJK SC'; }
.pdf:lang(zh-TW) .sans { font-family: Inter, ui-sans-serif, -apple-system, BlinkMacSystemFont, "Segoe UI", Helvetica, "Apple Color Emoji", Arial, sans-serif, "Segoe UI Emoji", "Segoe UI Symbol", 'Twemoji', 'Noto Color Emoji', 'Noto Sans CJK TC'; }
.pdf:lang(ko-KR) .sans { font-family: Inter, ui-sans-serif, -apple-system, BlinkMacSystemFont, "Segoe UI", Helvetica, "Apple Color Emoji", Arial, sans-serif, "Segoe UI Emoji", "Segoe UI Symbol", 'Twemoji', 'Noto Color Emoji', 'Noto Sans CJK KR'; }
.pdf .code { font-family: Source Code Pro, "SFMono-Regular", Menlo, Consolas, "PT Mono", "Liberation Mono", Courier, monospace, 'Twemoji', 'Noto Color Emoji', 'Noto Sans Mono CJK JP'; }
.pdf:lang(zh-CN) .code { font-family: Source Code Pro, "SFMono-Regular", Menlo, Consolas, "PT Mono", "Liberation Mono", Courier, monospace, 'Twemoji', 'Noto Color Emoji', 'Noto Sans Mono CJK SC'; }
.pdf:lang(zh-TW) .code { font-family: Source Code Pro, "SFMono-Regular", Menlo, Consolas, "PT Mono", "Liberation Mono", Courier, monospace, 'Twemoji', 'Noto Color Emoji', 'Noto Sans Mono CJK TC'; }
.pdf:lang(ko-KR) .code { font-family: Source Code Pro, "SFMono-Regular", Menlo, Consolas, "PT Mono", "Liberation Mono", Courier, monospace, 'Twemoji', 'Noto Color Emoji', 'Noto Sans Mono CJK KR'; }
.pdf .serif { font-family: PT Serif, Lyon-Text, Georgia, ui-serif, serif, 'Twemoji', 'Noto Color Emoji', 'Noto Serif CJK JP'; }
.pdf:lang(zh-CN) .serif { font-family: PT Serif, Lyon-Text, Georgia, ui-serif, serif, 'Twemoji', 'Noto Color Emoji', 'Noto Serif CJK SC'; }
.pdf:lang(zh-TW) .serif { font-family: PT Serif, Lyon-Text, Georgia, ui-serif, serif, 'Twemoji', 'Noto Color Emoji', 'Noto Serif CJK TC'; }
.pdf:lang(ko-KR) .serif { font-family: PT Serif, Lyon-Text, Georgia, ui-serif, serif, 'Twemoji', 'Noto Color Emoji', 'Noto Serif CJK KR'; }
.pdf .mono { font-family: PT Mono, iawriter-mono, Nitti, Menlo, Courier, monospace, 'Twemoji', 'Noto Color Emoji', 'Noto Sans Mono CJK JP'; }
.pdf:lang(zh-CN) .mono { font-family: PT Mono, iawriter-mono, Nitti, Menlo, Courier, monospace, 'Twemoji', 'Noto Color Emoji', 'Noto Sans Mono CJK SC'; }
.pdf:lang(zh-TW) .mono { font-family: PT Mono, iawriter-mono, Nitti, Menlo, Courier, monospace, 'Twemoji', 'Noto Color Emoji', 'Noto Sans Mono CJK TC'; }
.pdf:lang(ko-KR) .mono { font-family: PT Mono, iawriter-mono, Nitti, Menlo, Courier, monospace, 'Twemoji', 'Noto Color Emoji', 'Noto Sans Mono CJK KR'; }
.highlight-default {
	color: rgba(55, 53, 47, 1);
}
.highlight-gray {
	color: rgba(120, 119, 116, 1);
	fill: rgba(120, 119, 116, 1);
}
.highlight-brown {
	color: rgba(159, 107, 83, 1);
	fill: rgba(159, 107, 83, 1);
}
.highlight-orange {
	color: rgba(217, 115, 13, 1);
	fill: rgba(217, 115, 13, 1);
}
.highlight-yellow {
	color: rgba(203, 145, 47, 1);
	fill: rgba(203, 145, 47, 1);
}
.highlight-teal {
	color: rgba(68, 131, 97, 1);
	fill: rgba(68, 131, 97, 1);
}
.highlight-blue {
	color: rgba(51, 126, 169, 1);
	fill: rgba(51, 126, 169, 1);
}
.highlight-purple {
	color: rgba(144, 101, 176, 1);
	fill: rgba(144, 101, 176, 1);
}
.highlight-pink {
	color: rgba(193, 76, 138, 1);
	fill: rgba(193, 76, 138, 1);
}
.highlight-red {
	color: rgba(212, 76, 71, 1);
	fill: rgba(212, 76, 71, 1);
}
.highlight-gray_background {
	background: rgba(241, 241, 239, 1);
}
.highlight-brown_background {
	background: rgba(244, 238, 238, 1);
}
.highlight-orange_background {
	background: rgba(251, 236, 221, 1);
}
.highlight-yellow_background {
	background: rgba(251, 243, 219, 1);
}
.highlight-teal_background {
	background: rgba(237, 243, 236, 1);
}
.highlight-blue_background {
	background: rgba(231, 243, 248, 1);
}
.highlight-purple_background {
	background: rgba(244, 240, 247, 0.8);
}
.highlight-pink_background {
	background: rgba(249, 238, 243, 0.8);
}
.highlight-red_background {
	background: rgba(253, 235, 236, 1);
}
.block-color-default {
	color: inherit;
	fill: inherit;
}
.block-color-gray {
	color: rgba(120, 119, 116, 1);
	fill: rgba(120, 119, 116, 1);
}
.block-color-brown {
	color: rgba(159, 107, 83, 1);
	fill: rgba(159, 107, 83, 1);
}
.block-color-orange {
	color: rgba(217, 115, 13, 1);
	fill: rgba(217, 115, 13, 1);
}
.block-color-yellow {
	color: rgba(203, 145, 47, 1);
	fill: rgba(203, 145, 47, 1);
}
.block-color-teal {
	color: rgba(68, 131, 97, 1);
	fill: rgba(68, 131, 97, 1);
}
.block-color-blue {
	color: rgba(51, 126, 169, 1);
	fill: rgba(51, 126, 169, 1);
}
.block-color-purple {
	color: rgba(144, 101, 176, 1);
	fill: rgba(144, 101, 176, 1);
}
.block-color-pink {
	color: rgba(193, 76, 138, 1);
	fill: rgba(193, 76, 138, 1);
}
.block-color-red {
	color: rgba(212, 76, 71, 1);
	fill: rgba(212, 76, 71, 1);
}
.block-color-gray_background {
	background: rgba(241, 241, 239, 1);
}
.block-color-brown_background {
	background: rgba(244, 238, 238, 1);
}
.block-color-orange_background {
	background: rgba(251, 236, 221, 1);
}
.block-color-yellow_background {
	background: rgba(251, 243, 219, 1);
}
.block-color-teal_background {
	background: rgba(237, 243, 236, 1);
}
.block-color-blue_background {
	background: rgba(231, 243, 248, 1);
}
.block-color-purple_background {
	background: rgba(244, 240, 247, 0.8);
}
.block-color-pink_background {
	background: rgba(249, 238, 243, 0.8);
}
.block-color-red_background {
	background: rgba(253, 235, 236, 1);
}
.select-value-color-pink { background-color: rgba(245, 224, 233, 1); }
.select-value-color-purple { background-color: rgba(232, 222, 238, 1); }
.select-value-color-green { background-color: rgba(219, 237, 219, 1); }
.select-value-color-gray { background-color: rgba(227, 226, 224, 1); }
.select-value-color-opaquegray { background-color: rgba(255, 255, 255, 0.0375); }
.select-value-color-orange { background-color: rgba(250, 222, 201, 1); }
.select-value-color-brown { background-color: rgba(238, 224, 218, 1); }
.select-value-color-red { background-color: rgba(255, 226, 221, 1); }
.select-value-color-yellow { background-color: rgba(253, 236, 200, 1); }
.select-value-color-blue { background-color: rgba(211, 229, 239, 1); }

.checkbox {
	display: inline-flex;
	vertical-align: text-bottom;
	width: 16;
	height: 16;
	background-size: 16px;
	margin-left: 2px;
	margin-right: 5px;
}

.checkbox-on {
	background-image: url("data:image/svg+xml;charset=UTF-8,%3Csvg%20width%3D%2216%22%20height%3D%2216%22%20viewBox%3D%220%200%2016%2016%22%20fill%3D%22none%22%20xmlns%3D%22http%3A%2F%2Fwww.w3.org%2F2000%2Fsvg%22%3E%0A%3Crect%20width%3D%2216%22%20height%3D%2216%22%20fill%3D%22%2358A9D7%22%2F%3E%0A%3Cpath%20d%3D%22M6.71429%2012.2852L14%204.9995L12.7143%203.71436L6.71429%209.71378L3.28571%206.2831L2%207.57092L6.71429%2012.2852Z%22%20fill%3D%22white%22%2F%3E%0A%3C%2Fsvg%3E");
}

.checkbox-off {
	background-image: url("data:image/svg+xml;charset=UTF-8,%3Csvg%20width%3D%2216%22%20height%3D%2216%22%20viewBox%3D%220%200%2016%2016%22%20fill%3D%22none%22%20xmlns%3D%22http%3A%2F%2Fwww.w3.org%2F2000%2Fsvg%22%3E%0A%3Crect%20x%3D%220.75%22%20y%3D%220.75%22%20width%3D%2214.5%22%20height%3D%2214.5%22%20fill%3D%22white%22%20stroke%3D%22%2336352F%22%20stroke-width%3D%221.5%22%2F%3E%0A%3C%2Fsvg%3E");
}
	
</style></head><body><article id="c51c0922-967f-4f12-bc0f-e69b2fda9aae" class="page sans"><header><h1 class="page-title">React snippets extension</h1></header><div class="page-body"><p id="f7dc5eda-111c-4773-9cc4-ca5d6b4edad4" class=""><a href="https://github.com/evertonvargas/react-snippets-extension">https://github.com/evertonvargas/react-snippets-extension</a></p><p id="700aacd0-a8b3-46ba-80c3-d9cb5b2a70fb" class="">
</p><p id="2f0e5e6c-0205-48a1-ad91-5e3f52b7a9b1" class="">start + modifier + (action || hook) + variant</p><h2 id="9e7c97db-d510-42fe-bb58-a3c58bb11e86" class="">Starts with</h2><ul id="816a5e95-acf9-45fe-98f1-a757e22b8a42" class="bulleted-list"><li style="list-style-type:disc">r  → Refers to React.js environment;</li></ul><ul id="d8cf7227-ecbd-41ab-a2ec-5fde0ed77cbc" class="bulleted-list"><li style="list-style-type:disc">rn → Refers to <strong><span style="border-bottom:0.05em solid">R</span></strong>eact <strong><span style="border-bottom:0.05em solid">N</span></strong>ative environment;</li></ul><ul id="57fc5a60-df65-4116-9afb-e8a68858217a" class="bulleted-list"><li style="list-style-type:disc">js → JavaScript.</li></ul><h2 id="027e2785-acbf-486f-9cea-9ba3dc7d6621" class="">Modifiers </h2><ul id="41d4ee6c-863c-4621-8ddd-81c0d00f9d60" class="bulleted-list"><li style="list-style-type:disc">e → export;</li></ul><ul id="05da5e53-d93f-46d1-9147-0e72c9dfc56d" class="bulleted-list"><li style="list-style-type:disc">ed → export default;</li></ul><ul id="c3fb78f6-fcce-4c89-8aa4-c46b6d23bd38" class="bulleted-list"><li style="list-style-type:disc">a → async.</li></ul><h2 id="1e19dc4f-8b3f-4774-b8c5-48143f0f450b" class="">Action</h2><ul id="f2d38793-8dd3-49bf-8ceb-93e7cc7f4000" class="bulleted-list"><li style="list-style-type:disc">f → function;</li></ul><ul id="26b2b719-6a13-4be1-b79b-43e0e855c4cf" class="bulleted-list"><li style="list-style-type:disc">c → função com constante;</li></ul><ul id="1c10429d-277a-4855-b895-5f369a2b81a3" class="bulleted-list"><li style="list-style-type:disc">s → styles;</li></ul><ul id="108c1f56-5fea-4e70-9c87-4a7c52014f5e" class="bulleted-list"><li style="list-style-type:disc">sb → style block;</li></ul><ul id="d1381ed0-1132-40c3-901d-d85597e9b96f" class="bulleted-list"><li style="list-style-type:disc">sc → styled components.</li></ul><h2 id="e0135c89-72be-4d2e-862c-717b8bb55b94" class="">Variants (if available)</h2><ul id="6d71118a-3d23-4009-b455-12eae2ed1ee3" class="bulleted-list"><li style="list-style-type:disc">n → nested (set component name same as folder name);</li></ul><ul id="464a7408-7f1c-41c3-8523-f080ac3d566f" class="bulleted-list"><li style="list-style-type:disc">t → use the TypeScript variant.</li></ul><h1 id="aedd2c14-16b6-4353-a16a-762fb24eb2d3" class="">Using with React</h1><p id="6b21e9ff-d507-4015-a1d0-177c99ba31eb" class="">Everything related to <span style="border-bottom:0.05em solid">R</span>eact environment will use the <code>r</code> prefix.</p><h2 id="81bfbf50-dd3c-4d0b-8499-836500a7a929" class="">Specials Variant</h2><p id="c287e62a-7935-42a0-ab35-ecbd4e374586" class="">These modifiers, at the moment, are available only within a React environment. They <span style="border-bottom:0.05em solid">must be added at the end</span> of the <em><em><em><em><em><em><em><em><em><em><em><em><em><em>snippet query</em></em></em></em></em></em></em></em></em></em></em></em></em></em> and <span style="border-bottom:0.05em solid">must be in alphabetical order</span>.</p><ul id="f7ee61bd-9ecc-4050-a351-ebc81717fa1b" class="bulleted-list"><li style="list-style-type:disc">n → It means that your current <em><em><em><em><em><em>.tsx</em></em></em></em></em></em>/<em><em><em><em>.jsx</em></em></em></em> file is nested into a folder. If used it will automatically set the created function’s name to be the same as the <span style="border-bottom:0.05em solid">folder above</span> (<em>father</em>) your file.</li></ul><ul id="45f79491-f83e-41e1-9eeb-01e1bad15c03" class="bulleted-list"><li style="list-style-type:disc">t → This indicates that you want to use the TypeScript variant, if exists, of this snippet. </li></ul><h2 id="f1bd993a-9294-4cce-8911-28e1a5a81ccb" class="">Hooks</h2><p id="9968f645-e8d6-43e5-a581-eaad699541b4" class="">Can replace the modifiers and starts with <strong><em>u</em></strong><em> (use)</em> followed by the first letter of the hook’s name:</p><table id="13b84e9e-c59f-4442-8f2d-1dc982537a31" class="simple-table"><tbody><tr id="ef26d3c2-05e8-47c1-b2b2-9a8d64c9edfe"><td id="HGkr" class="" style="width:70px">Snippet</td><td id="B`SR" class="" style="width:146px">Content</td></tr><tr id="2772d4ee-4f2a-424d-a7b0-f6ae7546ddbd"><td id="HGkr" class="" style="width:70px"><code>rue</code></td><td id="B`SR" class="" style="width:146px">React <span style="border-bottom:0.05em solid"><strong>u</strong></span>se<span style="border-bottom:0.05em solid"><strong>E</strong></span>ffect</td></tr><tr id="a7a0c626-c946-47ec-a32f-7de74d67a0a3"><td id="HGkr" class="" style="width:70px"><code>rus</code></td><td id="B`SR" class="" style="width:146px">React <span style="border-bottom:0.05em solid"><strong>u</strong></span>se<span style="border-bottom:0.05em solid"><strong>S</strong></span>tate</td></tr></tbody></table><h2 id="447c7b44-bd37-40e7-b454-542caa213789" class="">Exporting Components</h2><p id="81b7bbdd-ab1b-405a-b6a6-0d1d7875ac32" class="">By default, when you use the snippet to create/export a function/component it will use the current <em><em><em><em><em><em>.tsx</em></em></em></em></em></em>/<em><em><em><em>.jsx</em></em></em></em> to set its name. If you want it to use the folder’s name it is nested in, use the<strong><em><strong><em> n</em></strong></em></strong> variant, as you can see <a href="https://www.notion.so/React-snippets-extension-c51c0922967f4f12bc0fe69b2fda9aae"><span style="border-bottom:0.05em solid">here</span></a></p><h3 id="0adcf7e5-7eef-4a71-a4fe-a00feb9c3986" class="">React ( .js and Native)</h3><p id="c4a75d4a-f092-4ea3-a378-f738f119c28b" class="">When you are creating a new component you can use the following snippets to automatically generate its structure: </p><table id="c0ae4da6-17de-4605-acd4-a39bb8c3f620" class="simple-table"><thead class="simple-table-header"><tr id="331092b8-3eea-406d-b36b-0a1283295397"><th id="`x~R" class="simple-table-header-color simple-table-header" style="width:80px">Snippet</th><th id="yBFX" class="simple-table-header-color simple-table-header" style="width:373px">Content</th></tr></thead><tbody><tr id="96462fa2-92e2-4ca3-8fa6-1aebc9da29f3"><th id="`x~R" class="simple-table-header-color simple-table-header" style="width:80px"><code>ref</code></th><td id="yBFX" class="" style="width:373px"><span style="border-bottom:0.05em solid">R</span>eact <span style="border-bottom:0.05em solid">E</span>xport <span style="border-bottom:0.05em solid">F</span>unction</td></tr><tr id="95c2ef7e-92d7-4fe5-9937-fe383e1e7569"><th id="`x~R" class="simple-table-header-color simple-table-header" style="width:80px"><code>redf</code></th><td id="yBFX" class="" style="width:373px"><span style="border-bottom:0.05em solid">R</span>eact <span style="border-bottom:0.05em solid">E</span>xport <span style="border-bottom:0.05em solid">D</span>efault <span style="border-bottom:0.05em solid">F</span>unction</td></tr><tr id="865f2758-5874-4da6-af55-f4e7fb6c1fa2"><th id="`x~R" class="simple-table-header-color simple-table-header" style="width:80px"><code>recf</code></th><td id="yBFX" class="" style="width:373px"><span style="border-bottom:0.05em solid">R</span>eact <span style="border-bottom:0.05em solid">E</span>xport <span style="border-bottom:0.05em solid">C</span>onst <span style="border-bottom:0.05em solid">F</span>unction</td></tr><tr id="634c5306-70d6-460a-8ca5-e73fdadef321"><th id="`x~R" class="simple-table-header-color simple-table-header" style="width:80px"><code>redcf</code></th><td id="yBFX" class="" style="width:373px"><span style="border-bottom:0.05em solid">R</span>eact <span style="border-bottom:0.05em solid">E</span>xport Default <span style="border-bottom:0.05em solid">C</span>onst <span style="border-bottom:0.05em solid">F</span>unction</td></tr></tbody></table><p id="fddb0314-d0db-4291-9cb8-2a00b5b4e5e7" class="">If you need a typescript function with a Props Interface, you can just add a <strong><em>t</em></strong> to the end of the snippet:</p><table id="507e4ad2-908b-43f6-b8ec-f0e8e5bcf8f8" class="simple-table"><thead class="simple-table-header"><tr id="faedbe02-803d-48df-8bf1-8335fe1f0c0d"><th id="pKVE" class="simple-table-header-color simple-table-header" style="width:72px">Snippet</th><th id="V?IT" class="simple-table-header-color simple-table-header" style="width:378.609375px">Content</th></tr></thead><tbody><tr id="4bf21c1c-3afb-4829-9ac1-d48b7cbabc76"><th id="pKVE" class="simple-table-header-color simple-table-header" style="width:72px"><code>reft</code></th><td id="V?IT" class="" style="width:378.609375px"><span style="border-bottom:0.05em solid">R</span>eact <span style="border-bottom:0.05em solid">E</span>xport <span style="border-bottom:0.05em solid">F</span>unction (TypeScript)</td></tr><tr id="74d2a79d-73a1-4762-a6e6-437770c8ce1f"><th id="pKVE" class="simple-table-header-color simple-table-header" style="width:72px"><code>redft</code></th><td id="V?IT" class="" style="width:378.609375px"><span style="border-bottom:0.05em solid">R</span>eact <span style="border-bottom:0.05em solid">E</span>xport <span style="border-bottom:0.05em solid">D</span>efault <span style="border-bottom:0.05em solid">F</span>unction (TypeScript)</td></tr></tbody></table><p id="a024303b-1f48-4fb8-9267-11f955058611" class="">Now, if you want to go wild and use the <span style="border-bottom:0.05em solid"><em><em><em><em><em><em>n</em></em></em></em></em></em></span><em><em><em><em><em><em>ested</em></em></em></em></em></em> and <em><span style="border-bottom:0.05em solid">t</span></em><em><em><em><em><em><em><em><em>ypescript</em></em></em></em></em></em></em></em> variant <strong>AT THE SAME TIME</strong> (<em>insane…</em>) you should do this way:</p><table id="5a93632e-3b77-4431-9563-262b8549a69e" class="simple-table"><thead class="simple-table-header"><tr id="2b27ca0f-1eaf-4f7e-866b-4577c566b193"><th id="pKVE" class="simple-table-header-color simple-table-header" style="width:72px">Snippet</th><th id="V?IT" class="simple-table-header-color simple-table-header" style="width:378.609375px">Content</th></tr></thead><tbody><tr id="89327408-7dcc-47d9-9a4b-e59ad982c026"><th id="pKVE" class="simple-table-header-color simple-table-header" style="width:72px"><code>refnt</code></th><td id="V?IT" class="" style="width:378.609375px"><span style="border-bottom:0.05em solid">R</span>eact <span style="border-bottom:0.05em solid">E</span>xport <span style="border-bottom:0.05em solid">F</span>unction (<span style="border-bottom:0.05em solid">N</span>ested and <span style="border-bottom:0.05em solid">T</span>ypeScript)</td></tr><tr id="0af4e8d5-31a3-4a1c-aaa2-0daca7d15944"><th id="pKVE" class="simple-table-header-color simple-table-header" style="width:72px"><code>redfnt</code></th><td id="V?IT" class="" style="width:378.609375px"><span style="border-bottom:0.05em solid">R</span>eact <span style="border-bottom:0.05em solid">E</span>xport <span style="border-bottom:0.05em solid">D</span>efault <span style="border-bottom:0.05em solid">F</span>unction (<span style="border-bottom:0.05em solid">N</span>ested and <span style="border-bottom:0.05em solid">T</span>ypeScript)</td></tr></tbody></table><h3 id="c227e180-905f-44ca-9225-c00add6df4da" class="">React Native (only)</h3><p id="195cf5a0-9146-4c3a-a93b-27523428c68c" class="">Everything exclusively related to <span style="border-bottom:0.05em solid">R</span>eact <span style="border-bottom:0.05em solid">N</span>ative will use the <code>rn</code> prefix. When you are creating the styles of your component, you can use the following snippets to get it done quickly: </p><table id="4c4e8504-e232-4c80-a307-029813f483f6" class="simple-table"><thead class="simple-table-header"><tr id="74d57cb9-2690-41f6-85ad-5a37d7d78ba9"><th id="pKVE" class="simple-table-header-color simple-table-header" style="width:72px">Snippet</th><th id="V?IT" class="simple-table-header-color simple-table-header" style="width:378.609375px">Content</th></tr></thead><tbody><tr id="47797790-90d7-4453-916d-3eb5ee6899b4"><th id="pKVE" class="simple-table-header-color simple-table-header" style="width:72px"><code>rns</code></th><td id="V?IT" class="" style="width:378.609375px"><span style="border-bottom:0.05em solid">R</span>eact <span style="border-bottom:0.05em solid">N</span>ative <span style="border-bottom:0.05em solid">S</span>tyles</td></tr><tr id="23a6daab-96a2-4f4c-b29d-f12ccb12bcc0"><th id="pKVE" class="simple-table-header-color simple-table-header" style="width:72px"><code>rnsb</code></th><td id="V?IT" class="" style="width:378.609375px"><span style="border-bottom:0.05em solid">R</span>eact <span style="border-bottom:0.05em solid">N</span>ative <span style="border-bottom:0.05em solid">S</span>tyle <span style="border-bottom:0.05em solid">B</span>lock</td></tr><tr id="7d3a3730-ecb8-496a-be4c-e3feb40dc0b1"><th id="pKVE" class="simple-table-header-color simple-table-header" style="width:72px"><code>rnsc</code></th><td id="V?IT" class="" style="width:378.609375px"><span style="border-bottom:0.05em solid">R</span>eact <span style="border-bottom:0.05em solid">N</span>ative <span style="border-bottom:0.05em solid">S</span>tyled <span style="border-bottom:0.05em solid">C</span>omponents</td></tr></tbody></table><p id="f39b6bcd-cdb3-41e6-a229-40835b1067ff" class="">These only work on <em><em><em><em><em><em><em>.ts/.js</em></em></em></em></em></em></em> files, because are intended to be used as styles snippets</p><h1 id="e1d6f871-93b2-4a36-aac3-2fce341bced0" class="">Using with JavaScript/TypeScript</h1><p id="e3b4141f-59a5-4de3-aefb-fc20e16ce1f4" class="">Everything related to <span style="border-bottom:0.05em solid">J</span>ava<span style="border-bottom:0.05em solid">S</span>cript will use the <code>js</code> prefix. You can create functions,  arrow functions and </p><table id="b814ce18-6113-4472-a986-a6de83fa9b1d" class="simple-table"><thead class="simple-table-header"><tr id="a799325d-e0d3-471f-a540-1e436a8417e0"><th id="`x~R" class="simple-table-header-color simple-table-header" style="width:80px">Snippet</th><th id="yBFX" class="simple-table-header-color simple-table-header" style="width:373px">Content</th></tr></thead><tbody><tr id="1c53bad7-5606-47f6-83db-64b883ca198f"><th id="`x~R" class="simple-table-header-color simple-table-header" style="width:80px"><code>jsf</code></th><td id="yBFX" class="" style="width:373px"><span style="border-bottom:0.05em solid">J</span>ava<span style="border-bottom:0.05em solid">S</span>cript <span style="border-bottom:0.05em solid">F</span>unction</td></tr><tr id="5ff2d08e-fdfc-4183-a355-7fd35366ea1d"><th id="`x~R" class="simple-table-header-color simple-table-header" style="width:80px"><code>jscf</code></th><td id="yBFX" class="" style="width:373px"><span style="border-bottom:0.05em solid">J</span>ava<span style="border-bottom:0.05em solid">S</span>cript <span style="border-bottom:0.05em solid">C</span>onst <span style="border-bottom:0.05em solid">F</span>unction</td></tr><tr id="f1dbb1fd-9c41-4366-ab61-6e0b81a2264e"><th id="`x~R" class="simple-table-header-color simple-table-header" style="width:80px"><code>jsaf</code></th><td id="yBFX" class="" style="width:373px"><span style="border-bottom:0.05em solid">J</span>ava<span style="border-bottom:0.05em solid">S</span>cript <span style="border-bottom:0.05em solid">A</span>sync <span style="border-bottom:0.05em solid">F</span>unction</td></tr><tr id="3bfe60cb-552a-40a6-9baf-de5051daaae0"><th id="`x~R" class="simple-table-header-color simple-table-header" style="width:80px"><code>jsac</code></th><td id="yBFX" class="" style="width:373px"><span style="border-bottom:0.05em solid">J</span>ava<span style="border-bottom:0.05em solid">S</span>cript Async <span style="border-bottom:0.05em solid">C</span>onst <span style="border-bottom:0.05em solid">F</span>unction</td></tr></tbody></table><h2 id="99514866-d8f1-4c75-9b72-607c5815f82a" class="">JavaScript/TypeScript Utils</h2><p id="bc266d5e-e4dc-4a84-bf6c-6fff3f8d1a52" class="">This section still in development and will be completed in future updates. Right now you can use soma snippets to quickly access some built-in JavaScript methods.</p><h3 id="54f090fc-5782-4cca-89b8-d4573f80429b" class="">Fetch</h3><p id="1fed30ef-cc04-47d4-b5a3-a6161b4323b2" class="">Here you can see some snippets to create a <em><em><em><em><em><em>.fetch</em></em></em></em></em></em>. Te <em><span style="border-bottom:0.05em solid">a</span></em><em>sync</em> one will create a function that returns the value of the request.</p><table id="4da8cc93-5f3c-4692-bbff-dc60f6c5572d" class="simple-table"><tbody><tr id="6595f95b-b1a6-4d1d-adb7-681d9ae0d931"><td id="mP[\" class="">Snippet</td><td id="&lt;]Jt" class="">Content</td></tr><tr id="6292df18-b81a-47a2-8893-cfb8ad122372"><td id="mP[\" class=""><code>jsfetch</code></td><td id="&lt;]Jt" class=""><span style="border-bottom:0.05em solid">J</span>ava<span style="border-bottom:0.05em solid">S</span>cript <span style="border-bottom:0.05em solid">F</span>etch</td></tr><tr id="b6163a3f-98a3-464e-8fc5-2b8f8fb5dc79"><td id="mP[\" class=""><code>jsafetch</code></td><td id="&lt;]Jt" class=""><span style="border-bottom:0.05em solid">J</span>ava<span style="border-bottom:0.05em solid">S</span>cript <span style="border-bottom:0.05em solid">A</span>sync <span style="border-bottom:0.05em solid">F</span>etch</td></tr></tbody></table><p id="c26046b1-54ff-4195-a3de-cf8d6c1ac9d1" class="">
</p></div></article></body></html>
