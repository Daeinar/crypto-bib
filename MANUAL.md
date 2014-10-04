##Getting Started

###Required Files
You need to download and put in your paper's folder:

- One of the following files:
  - `abbrev0.bib`: for the most detailed entries;
  - `abbrev1.bib`: as `abbrev0.bib` but without days of conferences;
  - `abbrev2.bib`: as `abbrev0.bib` but with short names (for conferences, publishers, ...);
  - `abbrev3.bib`: a mix of `abbrev1.bib` and `abbrev2.bib`;
- One of the following files:
  - `crypto.bib`: the actual legacy database;
  - `crypto_crossref.bib`: as `crypto.bib` but lighter thanks to cross-references;
  - `crypto_custom.bib`: a custom version of one of the above files which can be created [here](http://cryptobib.di.ens.fr/init/default/custom).

You can also get all of the above files at once by downloading [crypto.zip](http://cryptobib.di.ens.fr/init/static/files/crypto.zip?attachment=).


###Usage
You just need to include the two files you have chosen. For example:

- `\bibliography{abbrev0, crypto}`
- `\bibliography{abbrev1, crypto}`
- `\bibliography{abbrev2, crypto_custom}`
- `\bibliography{abbrev3, crypto_crossref}`

If you use a version with cross-references, you may want to add the option `--min-crossrefs=1000` to bibtex to avoid having conferences in the bibliography.


###Labeling Conventions

Each label consists of a *Conference/Journal/Misc label* followed by a colon *(':')* followed an *Author label* and *the last 2 digits of the publication year*. In case of collisions, a different letter is added at the end of each label starting with *'a'*:

`<Conference/Journal/Misc label>:<Author label><2 last digits of publication year>[a/b/...]`

Here are some examples:

- `C:Shamir85`
- `TCC:KatVai11`
- `EC:ChaPhaPoi05`
- `FOCS:GNRS99`

###Conference/Journal/Misc Labels

####Conference Labels

| Acronym      | Label          |  Acronym     |  Label            |
| ------------ | -------------- | ------------ | ----------------- |
| ACISP        | **ACISP**      | ACM CCS      |  **CCS**          |
| ACNS         | **ACN**        | AFRICACRYPT  | **AFRICACRYPT**   |
| ASIACCS      | **ASIACCS**    | ASIACRYPT    | **AC**            |
| CANS         | **CANS**       | CHES         | **CHES**          |
| CQRE         | **CQRE**       | CRYPTO       | **C**             |
| CT-RSA       | **RSA**        | ESORICS      | **ESORICS**       |
| EUROCRYPT    | **EC**         | FC           | **FC**            |
| FCW          | **FCW**        | FOCS         | **FOCS**          |
| FSE          | **FSE**        | ICALP        | **ICALP**         |
| ICICS        | **ICICS**      | ICISC        | **ICISC**         |
| ICITS        | **ICITS**      | IEEE SP      | **SP**            |
| IMA          | **IMA**        | INDOCRYPT    | **INDOCRYPT**     |
| ISC          | **ISC**        | ITCS         | **ITCS**          |
| IWSEC        | **IWSEC**      | LATIN        | **LATIN**         |
| LATINCRYPT   | **LC**         | NDSS         | **NDSS**          |
| PAIRING      | **PAIRING**    | PKC          | **PKC**           |
| PODC         | **PODC**       | PROVSEC      | **PROVSEC**       |
| SAC          | **SAC**        | SCN          | **SCN**           |
| SODA         | **SODA**       | STOC         | **STOC**          |
| TCC          | **TCC**        | TRUSTBUS     | **TRUSTBUS**      |
| VIETCRYPT    | **VIETCRYPT**  | WISA         | **WISA**          |


####Journal Labels

| Acronym                | Label           |
| ---------------------- | --------------- |
| Journal of Cryptology  | **JC**          |


####Misc Labels

| Acronym               | Label           |
| --------------------- | --------------- |
| IACR ePRint           | **EPRINT**      |


###Author Labels

- **Single-author papers**: Author's last name;

  Examples:
  1. author = "Adi Shamir" &#10142; Shamir
  2. author = "Luke O'Connor" &#10142; OConnor

- **Papers with two or three authors**: First 3 letters of each author's last name;

  Examples:
  1. author = "Mihir Bellare and Phillip Rogaway" &#10142; BelRog
  2. author = "Michel Abdalla and Sara Miner and Chanathip Namprempre" &#10142; AbdMinNam

- **Papers with four or more authors**: First letter of each author's last name (up to 6);

  Examples:
  1. author = "Kamel Bentahar and Pooya Farshim and John Malone-Lee and Nigel P. Smart" &#10142; BFMS
  2. author = "Don Coppersmith and Jean-Sebastien Coron and Fran\c{c}ois Grieu and Shai Halevi and Charanjit S. Jutla and David Naccache and Julien P. Stern" &#10142; CCGHJN
