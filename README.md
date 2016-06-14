Mofang Indicators of Compromise
==================================

This repository contains the indicators of compromise for the Mofang group.

> Mofang (模仿, Mófang, to imitate) is a threat actor that almost certainly operates out of China and is probably government-affiliated.

Full report on the Mofang group can be found here:

 * [http://f0x.nl/mofang](http://f0x.nl/mofang) (short link)
 * [http://blog.fox-it.com/2016/06/15/mofang-a-politically-motivated-information-stealing-adversary/](http://blog.fox-it.com/2016/06/15/mofang-a-politically-motivated-information-stealing-adversary/)

### Available IOCs

| filename                                      | description                                                                                              |
|-----------------------------------------------|----------------------------------------------------------------------------------------------------------|
| *[domains.txt](domains.txt)*             | The C2 domains used by ShimRat and/o	r ShimRatReporter |
| *[ips.txt](ips.txt)* | The C2 IPs used by ShimRat and/or ShimRatReporter |
| *[hashes.txt](hashes.txt)* | The hashes for ShimRat and ShimRatReporter samples |
 
### Available signatures
| filename                                      | description                                                                                              |
|-----------------------------------------------|----------------------------------------------------------------------------------------------------------|
| *[snort_signatures.txt](snort_signatures.txt)* | Contains Snort signatures to detect Shimrat and ShimRatReporter |
| *[yara_signatures.txt](yara_signatures.txt)* | Contains Yara signatures to detect Shimrat and ShimRatReporter |

### Availabe STIX Package
| filename                                      | description                                                                                              |
|-----------------------------------------------|------------------------------------------
| *[FoxIT_Mofang_STIX_1_2.xml](FoxIT_Mofang_STIX_1_2.xml)* | STIX package containing all the indicators and signatures |

### Shim Databases

As described in the report, ShimRat makes use of shims to obtain persistence on a system. The following files are the observed shim databases used by ShimRat. These files are the sdb's containing the fix information to inject the malicious ShimRat DLL into a process.

|filename                                                                                    |description|
|--------------------------------------------------------------------------------------------|--------|------------------------------------------------------------------------|
| *[{503EC3D3-165A-4770-B799-099D43B833EC}.sdb]({503EC3D3-165A-4770-B799-099D43B833EC}.sdb)* | The shim used for persistence on 32-bit Windows installations |
| *[{f8c4cc07-6dc4-418f-b72b-304fcdb64052}.sdb]({f8c4cc07-6dc4-418f-b72b-304fcdb64052}.sdb)* | The shim used for persistence on 64-bit Windows installations |

