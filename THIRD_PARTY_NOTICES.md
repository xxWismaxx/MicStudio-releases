# Third-party components

| Component | What it does in Mic Studio | License | Where |
|---|---|---|---|
| DPDFNet models (`dpdfnet2_48khz_hr`, `dpdfnet8_48khz_hr`), Ceva | The noise suppression network | Apache-2.0 | `models\`, [github.com/ceva-ip/DPDFNet](https://github.com/ceva-ip/DPDFNet), license in `models\DPDFNet-LICENSE.txt` |
| WeSpeaker CAM++ speaker model (`voice-print.onnx`), trained on VoxCeleb; ONNX export by sherpa-onnx | "Only my voice": the voice print | CC BY 4.0 (the VoxCeleb data's license, which WeSpeaker's models follow) | `models\`, [github.com/wenet-e2e/wespeaker](https://github.com/wenet-e2e/wespeaker), [k2-fsa/sherpa-onnx](https://github.com/k2-fsa/sherpa-onnx/releases/tag/speaker-recongition-models) |
| ONNX Runtime, Microsoft | Runs the network on the processor | MIT | NuGet `Microsoft.ML.OnnxRuntime` |
| WebView2, Microsoft | Draws the window | Microsoft Software License | NuGet `Microsoft.Web.WebView2` |
| usbip-win2 (installer, not shipped inside the app) | Plugs the virtual USB microphone into Windows; its drivers are signed by Microsoft | BSD-2-Clause | `drivers\`, [github.com/vadimgrn/usbip-win2](https://github.com/vadimgrn/usbip-win2), license in `drivers\usbip-win2-LICENSE.txt` |
| "Support me on Ko-fi" button, Ko-fi Labs | The button on the About page that opens the author's Ko-fi page | Ko-fi's creator kit, for linking to a Ko-fi page; Ko-fi's trademark | `ui\assets\kofi-button.png`, [more.ko-fi.com/brand-assets](https://more.ko-fi.com/brand-assets) |
| Lucide icons (refresh, download, info, settings) | Icons in the sidebar and on the About page | ISC | `ui\style.css`, [lucide.dev](https://lucide.dev) |
| GitHub mark (Octicons) and LinkedIn mark (Simple Icons) | The icons of the links to GitHub and LinkedIn | MIT (Octicons), CC0 (Simple Icons); the logos are their owners', used to link to them | `ui\style.css`, [github.com/primer/octicons](https://github.com/primer/octicons) |

The USB vendor id 0x1209 with product id 0x0001 is pid.codes' test id for open-source hardware; a release should
request its own product id from pid.codes.
