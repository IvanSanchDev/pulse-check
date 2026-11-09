# Third-party notices

The game page (index.html) is one packaged file. It contains copies of the open source libraries below. Most are under the MIT license, whose text is the same for all of them (only the copyright line differs) and is given once below. The MQTT.js bundle also carries code from many npm packages, most under the MIT license, two under the ISC license (inherits, lru-cache), one under the BSD-3-Clause license (ieee754) and one under the Apache License 2.0 (@jspm/core); the ISC, BSD-3-Clause and Apache texts follow the MIT text.

## React 18.3.1 and ReactDOM 18.3.1 (MIT)

Copyright (c) Facebook, Inc. and its affiliates.

(Taken from the license header at the top of each file inside the page. ReactDOM also carries a note that it includes code from Modernizr 3.0.0pre, a custom build, also under the MIT license.)

## MQTT.js 5.10.1 (MIT)

Copyright (c) 2015-2016 MQTT.js contributors

MQTT.js contributors listed at <https://github.com/mqttjs/MQTT.js#contributors>

Copyright 2011-2014 by Adam Rudd

(The minified file carries no copyright line of its own, so these lines are taken from the project's LICENSE.md at the v5.10.1 tag. The bundle also includes the packages below: ieee754, as its own bundled license note states, and @jspm/core and the npm packages listed after it, which the license note does not name.)

### ieee754, inside MQTT.js (BSD-3-Clause)

ieee754 by Feross Aboukhadijeh, <https://feross.org/opensource>, reaches the bundle through @jspm/core's browser Buffer (`@jspm/core/nodelibs/browser/buffer.js`). Its license text is given in full below.

### @jspm/core, inside MQTT.js (Apache License 2.0)

Copyright 2018-2021 Guy Bedford

The bundle's browser stand-ins for Node.js features (such as Buffer, process and events) come from @jspm/core, <https://github.com/jspm/jspm-core>. Its license text is given in full below.

### Packages bundled inside MQTT.js (all MIT unless marked)

The minified MQTT.js file names only ieee754 in its license comment, but it also contains code from the npm packages below. Each was found in the file by its own code or messages, and each is either a dependency MQTT.js 5.10.1 lists in its package.json or comes from @jspm/core, which MQTT.js's build (esbuild-plugin-polyfill-node) uses for the Node.js built-ins. The version given is the one whose LICENSE file was read at unpkg.com (the newest release inside the range MQTT.js 5.10.1 or the package that needs it declares); the copyright line is copied from that file. The MIT license text below applies to each of them, with its own copyright line.

#### mqtt-packet 9.0.2 (MIT)

Copyright (c) 2014-2017 mqtt-packet contributors (contributors listed at <https://github.com/mqttjs/mqtt-packet#contributors>). Source: <https://unpkg.com/mqtt-packet@9.0.2/LICENSE.md>

#### bl 6.1.6 (MIT)

Copyright (c) 2013-2019 bl contributors (contributors listed at <https://github.com/rvagg/bl#contributors>). Source: <https://unpkg.com/bl@6.1.6/LICENSE.md>

#### debug 4.4.3 (MIT)

Copyright (c) 2014-2017 TJ Holowaychuk <tj@vision-media.ca>

Copyright (c) 2018-2021 Josh Junon

Source: <https://unpkg.com/debug@4.4.3/LICENSE>

#### ms 2.1.3 (MIT), inside debug

Copyright (c) 2020 Vercel, Inc. Source: <https://unpkg.com/ms@2.1.3/license.md>

#### readable-stream 4.8.0 (MIT)

Copyright Node.js contributors. All rights reserved.

Copyright Joyent, Inc. and other Node contributors. All rights reserved. (for the parts that come from the joyent/node repository)

Source: <https://unpkg.com/readable-stream@4.8.0/LICENSE>

#### abort-controller 3.0.0 (MIT), inside readable-stream

Copyright (c) 2017 Toru Nagashima. Source: <https://unpkg.com/abort-controller@3.0.0/LICENSE>

#### process-nextick-args 2.0.1 (MIT)

Copyright (c) 2015 Calvin Metcalf. Source: <https://unpkg.com/process-nextick-args@2.0.1/license.md>

#### inherits 2.0.4 (ISC)

Copyright (c) Isaac Z. Schlueter. Source: <https://unpkg.com/inherits@2.0.4/LICENSE>. The ISC license text is given in full below.

#### lru-cache 10.4.3 (ISC)

Copyright (c) 2010-2023 Isaac Z. Schlueter and Contributors. Source: <https://unpkg.com/lru-cache@10.4.3/LICENSE>. The ISC license text is given in full below.

#### number-allocator 1.0.14 (MIT)

Copyright (c) 2021 Takatoshi Kondo. Source: <https://unpkg.com/number-allocator@1.0.14/LICENSE>

#### js-sdsl 4.3.0 (MIT), inside number-allocator

Copyright (c) 2021 Zilong Yao. Source: <https://unpkg.com/js-sdsl@4.3.0/LICENSE>

#### worker-timers 7.1.8 (MIT)

Copyright (c) 2024 Christoph Guttandin. Source: <https://unpkg.com/worker-timers@7.1.8/LICENSE>

#### worker-timers-broker 6.1.8 (MIT), inside worker-timers

Copyright (c) 2024 Christoph Guttandin. Source: <https://unpkg.com/worker-timers-broker@6.1.8/LICENSE>

#### worker-timers-worker 7.0.71 (MIT), inside worker-timers

Its built code is the small timer worker that worker-timers starts from a blob. Copyright (c) 2024 Christoph Guttandin. Source: <https://unpkg.com/worker-timers-worker@7.0.71/LICENSE>

#### fast-unique-numbers 8.0.13 (MIT), inside worker-timers-broker

Copyright (c) 2023 Christoph Guttandin. Source: <https://unpkg.com/fast-unique-numbers@8.0.13/LICENSE>

#### ws 8.22.2 (MIT), browser stub only

Only ws's `browser.js` (a function that throws "ws does not work in the browser") is in the bundle.

Copyright (c) 2011 Einar Otto Stangvik <einaros@gmail.com>

Copyright (c) 2013 Arnout Kazemier and contributors

Copyright (c) 2016 Luigi Pinca and contributors

Source: <https://unpkg.com/ws@8.22.2/LICENSE>

#### Node.js built-ins from @jspm/core (MIT)

The browser stand-ins for Buffer, events, process, punycode and string_decoder come from @jspm/core 2.1.0 (the version `esbuild-plugin-polyfill-node` 0.3.0 asks for with `^2.0.1`), whose files are built from the npm packages below. The copyright lines are those of the upstream packages' LICENSE files at the versions named, and the punycode version (2.1.0) is the one printed inside the bundle.

- buffer 6.0.3: Copyright (c) Feross Aboukhadijeh, and other contributors. Source: <https://unpkg.com/buffer@6.0.3/LICENSE>. Its base64 code is the base64-js package, and its number code is ieee754 (BSD-3-Clause, above).
- base64-js 1.5.1: Copyright (c) 2014 Jameson Little. Source: <https://unpkg.com/base64-js@1.5.1/LICENSE>
- events 3.3.0: Copyright Joyent, Inc. and other Node contributors. Source: <https://unpkg.com/events@3.3.0/LICENSE>
- process 0.11.10: Copyright (c) 2013 Roman Shtylman <shtylman@gmail.com>. Source: <https://unpkg.com/process@0.11.10/LICENSE>
- punycode 2.1.0: Copyright Mathias Bynens <https://mathiasbynens.be/>. Source: <https://unpkg.com/punycode@2.1.0/LICENSE-MIT.txt>
- string_decoder 1.3.0: Copyright Node.js contributors. All rights reserved. Also Copyright Joyent, Inc. and other Node contributors. All rights reserved. Source: <https://unpkg.com/string_decoder@1.3.0/LICENSE>

## qrcode-generator 1.4.4 (MIT)

Copyright (c) 2009 Kazuhiko Arase

URL: http://www.d-project.com/

(Taken from the license header of the file. "QR Code" is a registered trademark of DENSO WAVE INCORPORATED.)

## MIT license text

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.

## ISC license text (inherits, lru-cache)

Copyright (c) Isaac Z. Schlueter (inherits)

Copyright (c) 2010-2023 Isaac Z. Schlueter and Contributors (lru-cache)

Permission to use, copy, modify, and/or distribute this software for any
purpose with or without fee is hereby granted, provided that the above
copyright notice and this permission notice appear in all copies.

THE SOFTWARE IS PROVIDED "AS IS" AND THE AUTHOR DISCLAIMS ALL WARRANTIES
WITH REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF
MERCHANTABILITY AND FITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR
ANY SPECIAL, DIRECT, INDIRECT, OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES
WHATSOEVER RESULTING FROM LOSS OF USE, DATA OR PROFITS, WHETHER IN AN
ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS ACTION, ARISING OUT OF OR
IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.

## BSD-3-Clause license text (ieee754)

Copyright 2008 Fair Oaks Labs, Inc.

Redistribution and use in source and binary forms, with or without
modification, are permitted provided that the following conditions are met:

1. Redistributions of source code must retain the above copyright notice, this
list of conditions and the following disclaimer.

2. Redistributions in binary form must reproduce the above copyright notice,
this list of conditions and the following disclaimer in the documentation
and/or other materials provided with the distribution.

3. Neither the name of the copyright holder nor the names of its contributors
may be used to endorse or promote products derived from this software without
specific prior written permission.

THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.

## Apache License 2.0 text (@jspm/core)

```

                                 Apache License
                           Version 2.0, January 2004
                        https://www.apache.org/licenses/

   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION

   1. Definitions.

      "License" shall mean the terms and conditions for use, reproduction,
      and distribution as defined by Sections 1 through 9 of this document.

      "Licensor" shall mean the copyright owner or entity authorized by
      the copyright owner that is granting the License.

      "Legal Entity" shall mean the union of the acting entity and all
      other entities that control, are controlled by, or are under common
      control with that entity. For the purposes of this definition,
      "control" means (i) the power, direct or indirect, to cause the
      direction or management of such entity, whether by contract or
      otherwise, or (ii) ownership of fifty percent (50%) or more of the
      outstanding shares, or (iii) beneficial ownership of such entity.

      "You" (or "Your") shall mean an individual or Legal Entity
      exercising permissions granted by this License.

      "Source" form shall mean the preferred form for making modifications,
      including but not limited to software source code, documentation
      source, and configuration files.

      "Object" form shall mean any form resulting from mechanical
      transformation or translation of a Source form, including but
      not limited to compiled object code, generated documentation,
      and conversions to other media types.

      "Work" shall mean the work of authorship, whether in Source or
      Object form, made available under the License, as indicated by a
      copyright notice that is included in or attached to the work
      (an example is provided in the Appendix below).

      "Derivative Works" shall mean any work, whether in Source or Object
      form, that is based on (or derived from) the Work and for which the
      editorial revisions, annotations, elaborations, or other modifications
      represent, as a whole, an original work of authorship. For the purposes
      of this License, Derivative Works shall not include works that remain
      separable from, or merely link (or bind by name) to the interfaces of,
      the Work and Derivative Works thereof.

      "Contribution" shall mean any work of authorship, including
      the original version of the Work and any modifications or additions
      to that Work or Derivative Works thereof, that is intentionally
      submitted to Licensor for inclusion in the Work by the copyright owner
      or by an individual or Legal Entity authorized to submit on behalf of
      the copyright owner. For the purposes of this definition, "submitted"
      means any form of electronic, verbal, or written communication sent
      to the Licensor or its representatives, including but not limited to
      communication on electronic mailing lists, source code control systems,
      and issue tracking systems that are managed by, or on behalf of, the
      Licensor for the purpose of discussing and improving the Work, but
      excluding communication that is conspicuously marked or otherwise
      designated in writing by the copyright owner as "Not a Contribution."

      "Contributor" shall mean Licensor and any individual or Legal Entity
      on behalf of whom a Contribution has been received by Licensor and
      subsequently incorporated within the Work.

   2. Grant of Copyright License. Subject to the terms and conditions of
      this License, each Contributor hereby grants to You a perpetual,
      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
      copyright license to reproduce, prepare Derivative Works of,
      publicly display, publicly perform, sublicense, and distribute the
      Work and such Derivative Works in Source or Object form.

   3. Grant of Patent License. Subject to the terms and conditions of
      this License, each Contributor hereby grants to You a perpetual,
      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
      (except as stated in this section) patent license to make, have made,
      use, offer to sell, sell, import, and otherwise transfer the Work,
      where such license applies only to those patent claims licensable
      by such Contributor that are necessarily infringed by their
      Contribution(s) alone or by combination of their Contribution(s)
      with the Work to which such Contribution(s) was submitted. If You
      institute patent litigation against any entity (including a
      cross-claim or counterclaim in a lawsuit) alleging that the Work
      or a Contribution incorporated within the Work constitutes direct
      or contributory patent infringement, then any patent licenses
      granted to You under this License for that Work shall terminate
      as of the date such litigation is filed.

   4. Redistribution. You may reproduce and distribute copies of the
      Work or Derivative Works thereof in any medium, with or without
      modifications, and in Source or Object form, provided that You
      meet the following conditions:

      (a) You must give any other recipients of the Work or
          Derivative Works a copy of this License; and

      (b) You must cause any modified files to carry prominent notices
          stating that You changed the files; and

      (c) You must retain, in the Source form of any Derivative Works
          that You distribute, all copyright, patent, trademark, and
          attribution notices from the Source form of the Work,
          excluding those notices that do not pertain to any part of
          the Derivative Works; and

      (d) If the Work includes a "NOTICE" text file as part of its
          distribution, then any Derivative Works that You distribute must
          include a readable copy of the attribution notices contained
          within such NOTICE file, excluding those notices that do not
          pertain to any part of the Derivative Works, in at least one
          of the following places: within a NOTICE text file distributed
          as part of the Derivative Works; within the Source form or
          documentation, if provided along with the Derivative Works; or,
          within a display generated by the Derivative Works, if and
          wherever such third-party notices normally appear. The contents
          of the NOTICE file are for informational purposes only and
          do not modify the License. You may add Your own attribution
          notices within Derivative Works that You distribute, alongside
          or as an addendum to the NOTICE text from the Work, provided
          that such additional attribution notices cannot be construed
          as modifying the License.

      You may add Your own copyright statement to Your modifications and
      may provide additional or different license terms and conditions
      for use, reproduction, or distribution of Your modifications, or
      for any such Derivative Works as a whole, provided Your use,
      reproduction, and distribution of the Work otherwise complies with
      the conditions stated in this License.

   5. Submission of Contributions. Unless You explicitly state otherwise,
      any Contribution intentionally submitted for inclusion in the Work
      by You to the Licensor shall be under the terms and conditions of
      this License, without any additional terms or conditions.
      Notwithstanding the above, nothing herein shall supersede or modify
      the terms of any separate license agreement you may have executed
      with Licensor regarding such Contributions.

   6. Trademarks. This License does not grant permission to use the trade
      names, trademarks, service marks, or product names of the Licensor,
      except as required for reasonable and customary use in describing the
      origin of the Work and reproducing the content of the NOTICE file.

   7. Disclaimer of Warranty. Unless required by applicable law or
      agreed to in writing, Licensor provides the Work (and each
      Contributor provides its Contributions) on an "AS IS" BASIS,
      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
      implied, including, without limitation, any warranties or conditions
      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
      PARTICULAR PURPOSE. You are solely responsible for determining the
      appropriateness of using or redistributing the Work and assume any
      risks associated with Your exercise of permissions under this License.

   8. Limitation of Liability. In no event and under no legal theory,
      whether in tort (including negligence), contract, or otherwise,
      unless required by applicable law (such as deliberate and grossly
      negligent acts) or agreed to in writing, shall any Contributor be
      liable to You for damages, including any direct, indirect, special,
      incidental, or consequential damages of any character arising as a
      result of this License or out of the use or inability to use the
      Work (including but not limited to damages for loss of goodwill,
      work stoppage, computer failure or malfunction, or any and all
      other commercial damages or losses), even if such Contributor
      has been advised of the possibility of such damages.

   9. Accepting Warranty or Additional Liability. While redistributing
      the Work or Derivative Works thereof, You may choose to offer,
      and charge a fee for, acceptance of support, warranty, indemnity,
      or other liability obligations and/or rights consistent with this
      License. However, in accepting such obligations, You may act only
      on Your own behalf and on Your sole responsibility, not on behalf
      of any other Contributor, and only if You agree to indemnify,
      defend, and hold each Contributor harmless for any liability
      incurred by, or claims asserted against, such Contributor by reason
      of your accepting any such warranty or additional liability.

   END OF TERMS AND CONDITIONS
```
