# Copyright (C) 2017 The Dagger Authors.
#
# Licensed under the Apache License, Version 2.0 (the "License");
# you may not use this file except in compliance with the License.
# You may obtain a copy of the License at
#
# http://www.apache.org/licenses/LICENSE-2.0
#
# Unless required by applicable law or agreed to in writing, software
# distributed under the License is distributed on an "AS IS" BASIS,
# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
# See the License for the specific language governing permissions and
# limitations under the License.
#
# Description:
#   A skeletal application that demonstates wiring for an injected Application and Actiity.

package(default_visibility = ["//:src"])

android_library(
    name = "simple_lib",
    srcs = glob(["*.java"]),
    manifest = "AndroidManifest.xml",
    resource_files = glob(["res/**"]),
    deps = [
        "//:android",
        "//:android-support",
        "//:dagger_with_compiler",
        "//third_party:android_appcompat",
        "//third_party:android_support_annotations",
        "//third_party:android_support_fragment",
    ],
)

android_binary(
    name = "simple",
    manifest = "AndroidManifest.xml",
    manifest_merger = "legacy",
    deps = [
        ":simple_lib",
    ],
)
