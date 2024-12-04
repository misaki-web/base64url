# base64url

base64url is a Bash encoder/decoder for the base64url format
(base64 with an URL and filename safe alphabet). It's described
in the [RFC 4648 (section 5)](https://www.rfc-editor.org/rfc/rfc4648#section-5):

> This encoding may be referred to as "base64url".  This encoding
> should not be regarded as the same as the "base64" encoding and
> should not be referred to as only "base64".  Unless clarified
> otherwise, "base64" refers to the base 64 in the previous section.
> 
> This encoding is technically identical to the previous one, except
> for the 62:nd and 63:rd alphabet character, as indicated in Table 2.

Here's the table (Value / Encoding):

| V E  | V  E  | V  E  | V  E              |
| :--- | :--- | :--- | :--------------- |
|  0 A | 17 R | 34 i | 51 z             |
|  1 B | 18 S | 35 j | 52 0             |
|  2 C | 19 T | 36 k | 53 1             |
|  3 D | 20 U | 37 l | 54 2             |
|  4 E | 21 V | 38 m | 55 3             |
|  5 F | 22 W | 39 n | 56 4             |
|  6 G | 23 X | 40 o | 57 5             |
|  7 H | 24 Y | 41 p | 58 6             |
|  8 I | 25 Z | 42 q | 59 7             |
|  9 J | 26 a | 43 r | 60 8             |
| 10 K | 27 b | 44 s | 61 9             |
| 11 L | 28 c | 45 t | 62 - (minus)     |
| 12 M | 29 d | 46 u | 63 _ (underline) |
| 13 N | 30 e | 47 v |                  |
| 14 O | 31 f | 48 w |                  |
| 15 P | 32 g | 49 x |                  |
| 16 Q | 33 h | 50 y | (pad) =          |

## Installation

- Get the [latest version of `base64url` on GitHub](https://github.com/misaki-web/base64url/archive/refs/heads/main.zip).

- Unzip the downloaded archive and locate the folder `base64url-main`.

- Open a terminal and source the function: `source /path/to/base64url-main/base64url`

## Usage

`base64url` can now be invoked directly from the terminal. It supports encoding, decoding, and format conversions between base64 and base64url. For details and examples, run `base64url -h`.

## License

Copyright (C) 2023-2024  Misaki F. <https://github.com/misaki-web/base64url

This program is free software: you can redistribute it and/or modify
it under the terms of the GNU General Public License as published by
the Free Software Foundation, either version 3 of the License, or
(at your option) any later version.

This program is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
GNU General Public License for more details.

You should have received a copy of the GNU General Public License
along with this program.  If not, see <http://www.gnu.org/licenses/>.
