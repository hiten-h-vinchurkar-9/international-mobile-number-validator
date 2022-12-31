# International Mobile Number Validator

A simpler and smaller rewrite of Google's libphonenumber library in javascript.

![npm](https://img.shields.io/npm/v/international-mobile-number-validator)
![npm bundle size](https://img.shields.io/bundlephobia/min/international-mobile-number-validator)
![Snyk Vulnerabilities for npm package](https://img.shields.io/snyk/vulnerabilities/npm/international-mobile-number-validator)
![npm](https://img.shields.io/npm/dw/international-mobile-number-validator)
![NPM](https://img.shields.io/npm/l/international-mobile-number-validator)
[![FOSSA Status](https://app.fossa.com/api/projects/git%2Bgithub.com%2Fhiten-h-vinchurkar-9%2Finternational-mobile-number-validator.svg?type=shield)](https://app.fossa.com/projects/git%2Bgithub.com%2Fhiten-h-vinchurkar-9%2Finternational-mobile-number-validator?ref=badge_shield)

### Features
- Simple and easy to use in code.
- Smaller, compressed and lighweight in size. 
- Based on Google's powerful libphonenumber library.
- Zero dependency on other packages.

### Demo
https://re1.uk/_DviVO85Y

### Installation
Install the package via npm:
```sh
npm install --save international-mobile-number-validator
```
### Usage
The following is a simple phone information extraction example similar to what can be viewed on the official demo page.

##### Sample Code -
```sh
const imnv = require('international-mobile-number-validator');
let validateRequest = {"phoneNumber":"9028126381", "countryCode":"IN"};
let result = imnv.validatePhNumber(validateRequest.phoneNumber,validateRequest.countryCode);
console.log(result);
```

##### Sample Result - 
```sh
{
    parseResult: {
        country_code: 91,
        national_number: 9028126381,
        raw_input: '9028126381',
        country_code_source: 20
    },
    isPossibleNumer: true,
    isValidNumber: true,
    isValidNumberForRegion: true,
    phoneNumberRegion: 'IN',
    getNumberType: 'MOBILE'
}
```

##### Country Code Details - 
| Country Name | Carrier Code | Country Code |
| ------ | ------ | ------ |
 | Afghanistan | 93 | AF | 
 | Albania | 355 | AL | 
 | Algeria | 213 | DZ | 
 | American Samoa | 1 | AS | 
 | Andorra | 376 | AD | 
 | Angola | 244 | AO | 
 | Anguilla | 1 | AI | 
 | Antigua and Barbuda | 1 | AG | 
 | Argentina | 54 | AR | 
 | Armenia | 374 | AM | 
 | Aruba | 297 | AW | 
 | Australia | 61 | AU | 
 | Austria | 43 | AT | 
 | Azerbaijan | 994 | AZ | 
 | Bahamas | 1 | BS | 
 | Bahrain | 973 | BH | 
 | Bangladesh | 880 | BD | 
 | Barbados | 1 | BB | 
 | Belarus | 375 | BY | 
 | Belgium | 32 | BE | 
 | Belize | 501 | BZ | 
 | Benin | 229 | BJ | 
 | Bermuda | 1 | BM | 
 | Bhutan | 975 | BT | 
 | Bolivia | 591 | BO | 
 | Bosnia and Herzegovina | 387 | BA | 
 | Botswana | 267 | BW | 
 | Brazil | 55 | BR | 
 | British Indian Ocean Territory | 246 | IO | 
 | British Virgin Islands | 1 | VG | 
 | Brunei | 673 | BN | 
 | Bulgaria | 359 | BG | 
 | Burkina Faso | 226 | BF | 
 | Burundi | 257 | BI | 
 | Cambodia | 855 | KH | 
 | Cameroon | 237 | CM | 
 | Canada | 1 | CA | 
 | Cape Verde | 238 | CV | 
 | Caribbean Netherlands | 599 | BQ | 
 | Cayman Islands | 1 | KY | 
 | Central African Republic | 236 | CF | 
 | Chad | 235 | TD | 
 | Chile | 56 | CL | 
 | China | 86 | CN | 
 | Christmas Island | 61 | CX | 
 | Cocos Islands | 61 | CC | 
 | Colombia | 57 | CO | 
 | Comoros | 269 | KM | 
 | Congo (DRC) | 243 | CD | 
 | Congo (Republic) | 242 | CG | 
 | Cook Islands | 682 | CK | 
 | Costa Rica | 506 | CR | 
 | Côte d’Ivoire | 225 | CI | 
 | Croatia | 385 | HR | 
 | Cuba | 53 | CU | 
 | Curaçao | 599 | CW | 
 | Cyprus | 357 | CY | 
 | Czech Republic | 420 | CZ | 
 | Denmark | 45 | DK | 
 | Djibouti | 253 | DJ | 
 | Dominica | 1 | DM | 
 | Dominican Republic | 1 | DO | 
 | Ecuador | 593 | EC | 
 | Egypt | 20 | EG | 
 | El Salvador | 503 | SV | 
 | Equatorial Guinea | 240 | GQ | 
 | Eritrea | 291 | ER | 
 | Estonia | 372 | EE | 
 | Ethiopia | 251 | ET | 
 | Falkland Islands | 500 | FK | 
 | Faroe Islands | 298 | FO | 
 | Fiji | 679 | FJ | 
 | Finland | 358 | FI | 
 | France | 33 | FR | 
 | French Guiana | 594 | GF | 
 | French Polynesia | 689 | PF | 
 | Gabon | 241 | GA | 
 | Gambia | 220 | GM | 
 | Georgia | 995 | GE | 
 | Germany | 49 | DE | 
 | Ghana | 233 | GH | 
 | Gibraltar | 350 | GI | 
 | Greece | 30 | GR | 
 | Greenland | 299 | GL | 
 | Grenada | 1 | GD | 
 | Guadeloupe | 590 | GP | 
 | Guam | 1 | GU | 
 | Guatemala | 502 | GT | 
 | Guernsey | 44 | GG | 
 | Guinea | 224 | GN | 
 | Guinea-Bissau | 245 | GW | 
 | Guyana | 592 | GY | 
 | Haiti | 509 | HT | 
 | Honduras | 504 | HN | 
 | Hong Kong | 852 | HK | 
 | Hungary | 36 | HU | 
 | Iceland | 354 | IS | 
 | India | 91 | IN | 
 | Indonesia | 62 | ID | 
 | Iran | 98 | IR | 
 | Iraq | 964 | IQ | 
 | Ireland | 353 | IE | 
 | Isle of Man | 44 | IM | 
 | Israel | 972 | IL | 
 | Italy | 39 | IT | 
 | Jamaica | 1 | JM | 
 | Japan | 81 | JP | 
 | Jersey | 44 | JE | 
 | Jordan | 962 | JO | 
 | Kazakhstan | 7 | KZ | 
 | Kenya | 254 | KE | 
 | Kiribati | 686 | KI | 
 | Kosovo | 383 | XK | 
 | Kuwait | 965 | KW | 
 | Kyrgyzstan | 996 | KG | 
 | Laos | 856 | LA | 
 | Latvia  | 371 | LV | 
 | Lebanon | 961 | LB | 
 | Lesotho | 266 | LS | 
 | Liberia | 231 | LR | 
 | Libya | 218 | LY | 
 | Liechtenstein | 423 | LI | 
 | Lithuania | 370 | LT | 
 | Luxembourg | 352 | LU | 
 | Macau | 853 | MO | 
 | Macedonia | 389 | MK | 
 | Madagascar | 261 | MG | 
 | Malawi | 265 | MW | 
 | Malaysia | 60 | MY | 
 | Maldives | 960 | MV | 
 | Mali | 223 | ML | 
 | Malta | 356 | MT | 
 | Marshall Islands | 692 | MH | 
 | Martinique | 596 | MQ | 
 | Mauritania | 222 | MR | 
 | Mauritius | 230 | MU | 
 | Mayotte | 262 | YT | 
 | Mexico | 52 | MX | 
 | Micronesia | 691 | FM | 
 | Moldova | 373 | MD | 
 | Monaco | 377 | MC | 
 | Mongolia | 976 | MN | 
 | Montenegro | 382 | ME | 
 | Montserrat | 1 | MS | 
 | Morocco | 212 | MA | 
 | Mozambique | 258 | MZ | 
 | Myanmar | 95 | MM | 
 | Namibia | 264 | NA | 
 | Nauru | 674 | NR | 
 | Nepal | 977 | NP | 
 | Netherlands | 31 | NL | 
 | New Caledonia | 687 | NC | 
 | New Zealand | 64 | NZ | 
 | Nicaragua | 505 | NI | 
 | Niger | 227 | NE | 
 | Nigeria | 234 | NG | 
 | Niue | 683 | NU | 
 | Norfolk Island | 672 | NF | 
 | North Korea | 850 | KP | 
 | Northern Mariana Islands | 1 | MP | 
 | Norway | 47 | NO | 
 | Oman | 968 | OM | 
 | Pakistan | 92 | PK | 
 | Palau | 680 | PW | 
 | Palestine | 970 | PS | 
 | Panama | 507 | PA | 
 | Papua New Guinea | 675 | PG | 
 | Paraguay | 595 | PY | 
 | Peru | 51 | PE | 
 | Philippines | 63 | PH | 
 | Poland | 48 | PL | 
 | Portugal | 351 | PT | 
 | Puerto Rico | 1 | PR | 
 | Qatar | 974 | QA | 
 | Réunion | 262 | RE | 
 | Romania | 40 | RO | 
 | Russia | 7 | RU | 
 | Rwanda | 250 | RW | 
 | Saint Barthélemy | 590 | BL | 
 | Saint Helena | 290 | SH | 
 | Saint Kitts and Nevis | 1 | KN | 
 | Saint Lucia | 1 | LC | 
 | Saint Martin | 590 | MF | 
 | Saint Pierre and Miquelon | 508 | PM | 
 | Saint Vincent and the Grenadines | 1 | VC | 
 | Samoa | 685 | WS | 
 | San Marino | 378 | SM | 
 | São Tomé and Príncipe | 239 | ST | 
 | Saudi Arabia | 966 | SA | 
 | Senegal | 221 | SN | 
 | Serbia | 381 | RS | 
 | Seychelles | 248 | SC | 
 | Sierra Leone | 232 | SL | 
 | Singapore | 65 | SG | 
 | Sint Maarten | 1 | SX | 
 | Slovakia | 421 | SK | 
 | Slovenia | 386 | SI | 
 | Solomon Islands | 677 | SB | 
 | Somalia | 252 | SO | 
 | South Africa | 27 | ZA | 
 | South Korea | 82 | KR | 
 | South Sudan | 211 | SS | 
 | Spain | 34 | ES | 
 | Sri Lanka | 94 | LK | 
 | Sudan | 249 | SD | 
 | Suriname | 597 | SR | 
 | Svalbard and Jan Mayen | 47 | SJ | 
 | Swaziland | 268 | SZ | 
 | Sweden | 46 | SE | 
 | Switzerland | 41 | CH | 
 | Syria | 963 | SY | 
 | Taiwan | 886 | TW | 
 | Tajikistan | 992 | TJ | 
 | Tanzania | 255 | TZ | 
 | Thailand | 66 | TH | 
 | Timor-Leste | 670 | TL | 
 | Togo | 228 | TG | 
 | Tokelau | 690 | TK | 
 | Tonga | 676 | TO | 
 | Trinidad and Tobago | 1 | TT | 
 | Tunisia | 216 | TN | 
 | Turkey | 90 | TR | 
 | Turkmenistan | 993 | TM | 
 | Turks and Caicos Islands | 1 | TC | 
 | Tuvalu | 688 | TV | 
 | U.S. Virgin Islands | 1 | VI | 
 | Uganda | 256 | UG | 
 | Ukraine | 380 | UA | 
 | United Arab Emirates | 971 | AE | 
 | United Kingdom | 44 | GB | 
 | United States | 1 | US | 
 | Uruguay | 598 | UY | 
 | Uzbekistan | 998 | UZ | 
 | Vanuatu | 678 | VU | 
 | Vatican City  | 39 | VA | 
 | Venezuela | 58 | VE | 
 | Vietnam | 84 | VN | 
 | Wallis and Futuna | 681 | WF | 
 | Western Sahara | 212 | EH | 
 | Yemen | 967 | YE | 
 | Zambia | 260 | ZM | 
 | Zimbabwe | 263 | ZW | 
 | Åland Islands | 358 | AX | 

### References
- Google's [libphonenumber](https://github.com/googlei18n/libphonenumber) library.

### Licenses
[MIT](https://github.com/hiten-h-vinchurkar-9/international-mobile-number-validator/blob/main/LICENSE)

Google's `libphonenumber` is [licensed](https://github.com/google/libphonenumber/blob/master/LICENSE) under Apache 2.0.
[Apache 2](https://en.wikipedia.org/wiki/Apache_License#Licensing_conditions) does not require a derivative work of the software, or modifications to the original, to be distributed using the same license. Hence, this library is licensed under [MIT](LICENSE), which is [compatible](https://www.quora.com/Is-the-MIT-license-compatible-with-the-Apache-License-Version-2-APLv2) with Apache 2.
The Apache license is terminated if the user sues anyone over patent infringement related to the software covered by the license. This condition is added in order to prevent patent litigations.

[![FOSSA Status](https://app.fossa.com/api/projects/git%2Bgithub.com%2Fhiten-h-vinchurkar-9%2Finternational-mobile-number-validator.svg?type=small)](https://app.fossa.com/projects/git%2Bgithub.com%2Fhiten-h-vinchurkar-9%2Finternational-mobile-number-validator?ref=badge_small)
