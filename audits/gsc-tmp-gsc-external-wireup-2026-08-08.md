---
title: "GSC Audit: /tmp/gsc-external/wireup"
date: 2026-08-08
tags: [gsc, audit, security]
---

# 🔒 GSC Audit — /tmp/gsc-external/wireup

**Дата:** 08.08.2026 19:19  
**Путь:** `/tmp/gsc-external/wireup`  
**Всего находок:** 416  
**CRITICAL:** 178 | **HIGH:** 7 | **MEDIUM:** 176 | **LOW:** 30

## 📊 По детекторам

| Детектор | Находок |
|----------|--------|
| GS001 | 177 |
| GS018 | 174 |
| GS003 | 27 |
| GS025-debug_mode | 9 |
| GS015 | 8 |
| GS008 | 5 |
| GS000-LEGACY | 3 |
| GS021 | 3 |
| GS029 | 2 |
| GS004 | 2 |
| GS025-eval_usage | 2 |
| GS020 | 1 |
| GS007 | 1 |
| GS009 | 1 |
| Синхронный код в async | 1 |

## 🔴 Критические и важные

| Категория | Правило | Файл | Строка | Детали |
|-----------|--------|------|--------|--------|
| CRITICAL | GS001 | benchmark_results.csv | 2 | Found: 4317267146835166 |
| CRITICAL | GS001 | benchmark_results.csv | 2 | Found: 4799999999999995 |
| CRITICAL | GS001 | benchmark_results.csv | 6 | Found: 4799999999999995 |
| CRITICAL | GS001 | benchmark_results.csv | 8 | Found: 4528474655831 |
| CRITICAL | GS001 | benchmark_results.csv | 12 | Found: 4741097405905058 |
| CRITICAL | GS001 | benchmark_results.csv | 15 | Found: 4344348388814077 |
| CRITICAL | GS001 | benchmark_results.csv | 17 | Found: 5229734528787542 |
| CRITICAL | GS001 | benchmark_results.csv | 19 | Found: 5355046383813894 |
| CRITICAL | GS001 | benchmark_results.csv | 21 | Found: 4401716900029 |
| CRITICAL | GS001 | benchmark_results.csv | 23 | Found: 4460357657556 |
| CRITICAL | GS001 | benchmark_run_metrics.csv | 17 | Found: 6525365023643269 |
| CRITICAL | GS001 | benchmark_run_metrics.csv | 61 | Found: 4617664656968985 |
| CRITICAL | GS001 | benchmark_run_metrics.csv | 72 | Found: 4001849491584741 |
| CRITICAL | GS001 | benchmark_run_metrics.csv | 81 | Found: 4559811759614 |
| CRITICAL | GS001 | benchmark_run_metrics.csv | 89 | Found: 5380879049606436 |
| CRITICAL | GS001 | benchmark_run_metrics.csv | 100 | Found: 5212809320000815 |
| CRITICAL | GS001 | benchmark_run_metrics.csv | 108 | Found: 5445521353784974 |
| CRITICAL | GS001 | benchmark_run_metrics.csv | 109 | Found: 4180682100990365 |
| CRITICAL | GS001 | benchmark_run_metrics.csv | 120 | Found: 4213796148528004 |
| CRITICAL | GS001 | benchmark_run_metrics.csv | 122 | Found: 4928705359998276 |
| CRITICAL | GS001 | benchmark_run_metrics.csv | 126 | Found: 4652834969965625 |
| CRITICAL | GS001 | benchmark_run_metrics.csv | 133 | Found: 4352596480545161 |
| CRITICAL | GS001 | benchmark_run_metrics.csv | 141 | Found: 344136417996197 |
| CRITICAL | GS001 | benchmark_run_metrics.csv | 145 | Found: 4382585718248 |
| CRITICAL | GS001 | benchmark_run_metrics.csv | 148 | Found: 5150423949962715 |
| CRITICAL | GS001 | benchmark_run_metrics.csv | 150 | Found: 4802895309985615 |
| CRITICAL | GS001 | benchmark_run_metrics.csv | 157 | Found: 4451085565693 |
| CRITICAL | GS001 | benchmark_run_metrics.csv | 161 | Found: 5523205552900942 |
| CRITICAL | GS001 | benchmark_run_metrics.csv | 165 | Found: 6590358339136833 |
| CRITICAL | GS001 | benchmark_run_metrics.csv | 168 | Found: 4953069209414 |
| CRITICAL | GS001 | benchmark_run_metrics.csv | 169 | Found: 5341773131158214 |
| CRITICAL | GS001 | benchmark_run_metrics.csv | 181 | Found: 4292982277363386 |
| CRITICAL | GS001 | benchmark_run_metrics.csv | 198 | Found: 5511396110014175 |
| CRITICAL | GS001 | benchmark_run_metrics.csv | 206 | Found: 349920900000143 |
| CRITICAL | GS001 | benchmark_run_metrics.csv | 213 | Found: 4919696939983176 |
| CRITICAL | GS001 | benchmark_run_metrics.csv | 217 | Found: 5245711311235493 |
| CRITICAL | GS001 | benchmark_run_metrics.csv | 229 | Found: 4493125848324389 |
| CRITICAL | GS001 | benchmark_run_metrics.csv | 237 | Found: 4687510481859766 |
| CRITICAL | GS001 | benchmark_run_metrics.csv | 240 | Found: 4999945197437 |
| CRITICAL | GS001 | benchmark_run_metrics.csv | 261 | Found: 5460914774641861 |
| CRITICAL | GS001 | benchmark_run_metrics.csv | 263 | Found: 4232625500008 |
| CRITICAL | GS001 | benchmark_run_metrics.csv | 264 | Found: 4320401024987226 |
| CRITICAL | GS001 | benchmark_run_metrics.csv | 272 | Found: 4094820078027204 |
| CRITICAL | GS001 | benchmark_run_metrics.csv | 281 | Found: 378749780000362 |
| CRITICAL | GS001 | benchmark_run_metrics.csv | 289 | Found: 5230781809422826 |
| CRITICAL | GS001 | benchmark_run_metrics.csv | 296 | Found: 4228217510745 |
| CRITICAL | GS001 | benchmark_run_metrics.csv | 296 | Found: 4763772973434967 |
| CRITICAL | GS001 | benchmark_run_metrics.csv | 301 | Found: 4369517151450555 |
| CRITICAL | GS001 | benchmark_run_metrics.csv | 305 | Found: 5192639557349974 |
| CRITICAL | GS001 | benchmark_run_metrics.csv | 312 | Found: 4088571548247277 |
| CRITICAL | GS001 | benchmark_run_metrics.csv | 325 | Found: 4435591118915412 |
| CRITICAL | GS001 | benchmark_run_metrics.csv | 329 | Found: 5107931100279374 |
| CRITICAL | GS001 | benchmark_run_metrics.csv | 340 | Found: 5313026559961145 |
| CRITICAL | GS001 | benchmark_run_metrics.csv | 344 | Found: 4080075546673697 |
| CRITICAL | GS001 | benchmark_run_metrics.csv | 349 | Found: 4228464171140423 |
| CRITICAL | GS001 | benchmark_run_metrics.csv | 353 | Found: 5595939971072027 |
| CRITICAL | GS001 | benchmark_run_metrics.csv | 357 | Found: 4544887384788913 |
| CRITICAL | GS001 | benchmark_run_metrics.csv | 360 | Found: 4301114702914508 |
| CRITICAL | GS001 | benchmark_run_metrics.csv | 361 | Found: 4533722789364092 |
| CRITICAL | GS001 | benchmark_run_metrics.csv | 377 | Found: 4797146359997 |
| CRITICAL | GS001 | benchmark_run_metrics.csv | 377 | Found: 5582822071006989 |
| CRITICAL | GS001 | benchmark_run_metrics.csv | 384 | Found: 4406948414620155 |
| CRITICAL | GS001 | benchmark_run_metrics.csv | 397 | Found: 4944112739463 |
| CRITICAL | GS001 | benchmark_run_metrics.csv | 405 | Found: 5531712287349037 |
| CRITICAL | GS001 | benchmark_run_metrics.csv | 408 | Found: 4289966411919957 |
| CRITICAL | GS001 | benchmark_run_metrics.csv | 421 | Found: 4600897405966202 |
| CRITICAL | GS001 | benchmark_run_metrics.csv | 425 | Found: 4668471601317 |
| CRITICAL | GS001 | benchmark_run_metrics.csv | 425 | Found: 5283863471185817 |
| CRITICAL | GS001 | benchmark_run_metrics.csv | 445 | Found: 4216970436403948 |
| CRITICAL | GS001 | benchmark_run_metrics.csv | 453 | Found: 4030024174672962 |
| CRITICAL | GS001 | benchmark_run_metrics.csv | 457 | Found: 5255362602336964 |
| CRITICAL | GS001 | benchmark_run_metrics.csv | 468 | Found: 5430791755480127 |
| CRITICAL | GS001 | benchmark_run_metrics.csv | 473 | Found: 5447358769676884 |
| CRITICAL | GS001 | benchmark_run_metrics.csv | 480 | Found: 376380471334514 |
| CRITICAL | GS001 | benchmark_run_metrics.csv | 481 | Found: 4843194247179 |
| CRITICAL | GS001 | benchmark_run_metrics.csv | 488 | Found: 4153532647739098 |
| CRITICAL | GS001 | benchmark_run_metrics.csv | 492 | Found: 370163126994157 |
| CRITICAL | GS001 | benchmark_run_metrics.csv | 493 | Found: 4469406132064928 |
| CRITICAL | GS001 | benchmark_run_metrics.csv | 501 | Found: 4081643852134255 |
| CRITICAL | GS001 | benchmark_run_metrics.csv | 517 | Found: 4064502828379613 |
| CRITICAL | GS001 | benchmark_run_metrics.csv | 526 | Found: 4695795919979 |
| CRITICAL | GS001 | benchmark_run_metrics.csv | 537 | Found: 6573373505589991 |
| CRITICAL | GS001 | benchmark_run_metrics.csv | 539 | Found: 4830452785645 |
| CRITICAL | GS001 | benchmark_run_metrics.csv | 545 | Found: 5498041295050522 |
| CRITICAL | GS001 | benchmark_run_metrics.csv | 554 | Found: 5181642360039405 |
| CRITICAL | GS001 | benchmark_run_metrics.csv | 560 | Found: 4250824366952602 |
| CRITICAL | GS001 | benchmark_run_metrics.csv | 565 | Found: 4258189320864942 |
| CRITICAL | GS001 | benchmark_run_metrics.csv | 566 | Found: 372793134003587 |
| CRITICAL | GS001 | benchmark_run_metrics.csv | 569 | Found: 5437071848992149 |
| CRITICAL | GS001 | benchmark_run_metrics.csv | 577 | Found: 4620078010048 |
| CRITICAL | GS001 | benchmark_run_metrics.csv | 589 | Found: 4324243353035313 |
| CRITICAL | GS001 | benchmark_run_metrics.csv | 593 | Found: 4651592940063 |
| CRITICAL | GS001 | benchmark_run_metrics.csv | 593 | Found: 5316236739915817 |
| CRITICAL | GS001 | benchmark_run_metrics.csv | 600 | Found: 4077221419041783 |
| CRITICAL | GS001 | benchmark_run_metrics.csv | 601 | Found: 5537661202415773 |
| CRITICAL | GS001 | benchmark_run_metrics.csv | 612 | Found: 5436953383929367 |
| CRITICAL | GS001 | benchmark_run_metrics.csv | 613 | Found: 4296423767377118 |
| CRITICAL | GS001 | benchmark_run_metrics.csv | 621 | Found: 340521798003465 |
| CRITICAL | GS001 | benchmark_run_metrics.csv | 632 | Found: 4022526866426614 |
| CRITICAL | GS001 | benchmark_run_metrics.csv | 637 | Found: 4065607637079955 |
| CRITICAL | GS001 | benchmark_run_metrics.csv | 661 | Found: 4549534473206829 |
| CRITICAL | GS001 | benchmark_run_metrics.csv | 665 | Found: 5121557035068988 |
| CRITICAL | GS001 | benchmark_run_metrics.csv | 669 | Found: 5497795385119473 |
| CRITICAL | GS001 | benchmark_run_metrics.csv | 684 | Found: 5524436110685271 |
| CRITICAL | GS001 | benchmark_run_metrics.csv | 689 | Found: 4322658960009 |
| CRITICAL | GS001 | benchmark_run_metrics.csv | 689 | Found: 4441991190624 |
| CRITICAL | GS001 | benchmark_run_metrics.csv | 697 | Found: 5214081062365408 |
| CRITICAL | GS001 | benchmark_run_metrics.csv | 709 | Found: 4515217767400816 |
| CRITICAL | GS001 | benchmark_run_metrics.csv | 713 | Found: 5535762577077624 |
| CRITICAL | GS001 | benchmark_run_metrics.csv | 733 | Found: 4312706453919202 |
| CRITICAL | GS001 | benchmark_run_metrics.csv | 734 | Found: 370042882001144 |
| CRITICAL | GS001 | benchmark_run_metrics.csv | 737 | Found: 5529595188422881 |
| CRITICAL | GS001 | benchmark_run_metrics.csv | 740 | Found: 4964989157115 |
| CRITICAL | GS001 | benchmark_run_metrics.csv | 757 | Found: 4179630523364062 |
| CRITICAL | GS001 | benchmark_run_metrics.csv | 761 | Found: 5306850419657008 |
| CRITICAL | GS001 | benchmark_run_metrics.csv | 793 | Found: 5491723583300723 |
| CRITICAL | GS001 | benchmark_run_metrics.csv | 800 | Found: 4146181892312835 |
| CRITICAL | GS001 | benchmark_run_metrics.csv | 805 | Found: 4724473185150149 |
| CRITICAL | GS001 | benchmark_run_metrics.csv | 828 | Found: 5424185525430167 |
| CRITICAL | GS001 | benchmark_run_metrics.csv | 829 | Found: 4244368306730366 |
| CRITICAL | GS001 | benchmark_run_metrics.csv | 833 | Found: 5561465710953233 |
| CRITICAL | GS001 | benchmark_run_metrics.csv | 842 | Found: 4546782090037595 |
| CRITICAL | GS001 | benchmark_run_metrics.csv | 852 | Found: 347165068000322 |
| CRITICAL | GS001 | benchmark_run_metrics.csv | 853 | Found: 4545634261563183 |
| CRITICAL | GS001 | benchmark_run_metrics.csv | 857 | Found: 5486192437654245 |
| CRITICAL | GS001 | benchmark_run_metrics.csv | 861 | Found: 4091662916340276 |
| CRITICAL | GS001 | benchmark_run_metrics.csv | 862 | Found: 374699079999118 |
| CRITICAL | GS001 | benchmark_run_metrics.csv | 877 | Found: 4663743458995124 |
| CRITICAL | GS001 | benchmark_run_metrics.csv | 888 | Found: 373050526037724 |
| CRITICAL | GS001 | benchmark_run_metrics.csv | 900 | Found: 4297637309087914 |
| CRITICAL | GS001 | benchmark_run_metrics.csv | 905 | Found: 5553961810097174 |
| CRITICAL | GS001 | benchmark_run_metrics.csv | 909 | Found: 4504682643434184 |
| CRITICAL | GS001 | benchmark_run_metrics.csv | 910 | Found: 4494474039966 |
| CRITICAL | GS001 | benchmark_run_metrics.csv | 913 | Found: 5555403543106616 |
| CRITICAL | GS001 | benchmark_run_metrics.csv | 920 | Found: 4150733884244783 |
| CRITICAL | GS001 | benchmark_run_metrics.csv | 925 | Found: 4412539639958974 |
| CRITICAL | GS001 | benchmark_run_metrics.csv | 927 | Found: 347613217918944 |
| CRITICAL | GS001 | benchmark_run_metrics.csv | 929 | Found: 5356803101085071 |
| CRITICAL | GS001 | benchmark_run_metrics.csv | 933 | Found: 5463852165679896 |
| CRITICAL | GS001 | benchmark_run_metrics.csv | 944 | Found: 4023071287390498 |
| CRITICAL | GS001 | benchmark_run_metrics.csv | 956 | Found: 4967122762755 |
| CRITICAL | GS001 | benchmark_run_metrics.csv | 977 | Found: 5580563422386767 |
| CRITICAL | GS001 | benchmark_run_metrics.csv | 986 | Found: 4295727019925835 |
| CRITICAL | GS001 | benchmark_run_metrics.csv | 997 | Found: 4632864183550742 |
| CRITICAL | GS001 | benchmark_run_metrics.csv | 998 | Found: 341112723996048 |
| CRITICAL | GS001 | benchmark_run_metrics.csv | 1001 | Found: 4239153667023422 |
| CRITICAL | GS001 | benchmark_run_metrics.csv | 1008 | Found: 4202547416697162 |
| CRITICAL | GS001 | benchmark_run_metrics.csv | 1009 | Found: 5535237966512991 |
| CRITICAL | GS001 | benchmark_run_metrics.csv | 1016 | Found: 4052398683156789 |
| CRITICAL | GS001 | benchmark_run_metrics.csv | 1021 | Found: 4148913083530992 |
| CRITICAL | GS001 | benchmark_run_metrics.csv | 1025 | Found: 370446425004047 |
| CRITICAL | GS001 | benchmark_run_metrics.csv | 1034 | Found: 4965707100054715 |
| CRITICAL | GS001 | benchmark_run_metrics.csv | 1053 | Found: 375846126000397 |
| CRITICAL | GS001 | benchmark_run_metrics.csv | 1080 | Found: 4216113176625969 |
| CRITICAL | GS001 | benchmark_run_metrics.csv | 1092 | Found: 5191278496028146 |
| CRITICAL | GS001 | benchmark_run_metrics.csv | 1093 | Found: 4149534653026896 |
| CRITICAL | GS001 | benchmark_run_metrics.csv | 1106 | Found: 4786612409952795 |
| CRITICAL | GS001 | benchmark_run_metrics.csv | 1110 | Found: 4779093350080075 |
| CRITICAL | GS001 | benchmark_run_metrics.csv | 1118 | Found: 347232621992589 |
| CRITICAL | GS001 | benchmark_run_metrics.csv | 1121 | Found: 4196028451100829 |
| CRITICAL | GS001 | benchmark_run_metrics.csv | 1129 | Found: 5528534365203155 |
| CRITICAL | GS001 | benchmark_run_metrics.csv | 1130 | Found: 5317597089888295 |
| CRITICAL | GS001 | benchmark_run_metrics.csv | 1141 | Found: 4023614818071182 |
| CRITICAL | GS001 | benchmark_run_metrics.csv | 1145 | Found: 5456328538047462 |
| CRITICAL | GS001 | benchmark_run_metrics.csv | 1165 | Found: 4231248376931085 |
| CRITICAL | GS001 | benchmark_run_metrics.csv | 1173 | Found: 4401716900029 |
| CRITICAL | GS001 | benchmark_run_metrics.csv | 1176 | Found: 371235971710158 |
| CRITICAL | GS001 | benchmark_run_metrics.csv | 1193 | Found: 5206737314310624 |
| CRITICAL | GS001 | benchmark_run_metrics.csv | 1201 | Found: 5385940561654645 |
| CRITICAL | GS001 | pyproject.toml | 79 | Found: "py310" |
| CRITICAL | GS001 | pyproject.toml | 86 | Found: "PT009" |
| CRITICAL | GS001 | pyproject.toml | 87 | Found: "TD003" |
| CRITICAL | GS001 | pyproject.toml | 95 | Found: "FA100" |
| CRITICAL | GS001 | pyproject.toml | 108 | Found: "EM101" |
| CRITICAL | GS001 | pyproject.toml | 110 | Found: "FA100" |
| CRITICAL | GS001 | pyproject.toml | 145 | Found: "UP015" |
| CRITICAL | GS001 | pyproject.toml | 154 | Found: "FA102" |
| CRITICAL | GS029 | aiohttp.py | 13 | Match: _container_key = "wireup_container" |
| HIGH | GS000-LEGACY | bench_runner.py | 71 | Match: URL_TEMPLATE = "http://127.0.0.1:{port}/{project}/{te |
| HIGH | GS000-LEGACY | bench_runner.py | 161 | Match:     url = f"http://127.0.0.1:{port}/healthz" |
| HIGH | GS000-LEGACY | bench_runner.py | 319 | Match:     url = f"http://127.0.0.1:{port}/assert-workload" |
| HIGH | GS008 | _wrapper_compiler.py | 60 | Match:     exec(code, namespace)  # noqa: S102 |
| HIGH | GS008 | factory_compiler.py | 281 | Match:             exec(compiled_code, namespace)  # noqa: S |
| HIGH | GS004 | _wrapper_compiler.py | 60 | Line 60: exec(code, namespace)  # noqa: S102 |
| HIGH | GS004 | factory_compiler.py | 281 | Line 281: exec(compiled_code, namespace)  # noqa: S102 |

## 📋 Все находки

| Кат. | Правило | Файл | Строка |
|------|--------|------|--------|
| M | GS018 | svcs_setup.py | 138 |
| M | GS018 | svcs_setup.py | 139 |
| M | GS018 | svcs_setup.py | 140 |
| M | GS018 | svcs_setup.py | 158 |
| M | GS018 | svcs_setup.py | 159 |
| M | GS018 | svcs_setup.py | 160 |
| M | GS018 | svcs_setup.py | 162 |
| M | GS018 | svcs_setup.py | 163 |
| M | GS018 | svcs_setup.py | 164 |
| M | GS018 | svcs_setup.py | 165 |
| M | GS018 | svcs_setup.py | 166 |
| M | GS018 | svcs_setup.py | 167 |
| M | GS018 | svcs_setup.py | 168 |
| M | GS018 | aioinject_setup.py | 32 |
| M | GS018 | aioinject_setup.py | 33 |
| M | GS018 | aioinject_setup.py | 34 |
| M | GS018 | aioinject_setup.py | 53 |
| M | GS018 | aioinject_setup.py | 54 |
| M | GS018 | aioinject_setup.py | 55 |
| M | GS018 | aioinject_setup.py | 57 |
| M | GS018 | aioinject_setup.py | 58 |
| M | GS018 | aioinject_setup.py | 59 |
| M | GS018 | aioinject_setup.py | 60 |
| M | GS018 | aioinject_setup.py | 61 |
| M | GS018 | aioinject_setup.py | 62 |
| M | GS018 | aioinject_setup.py | 63 |
| M | GS018 | dependency_injector_setup.py | 39 |
| M | GS018 | dependency_injector_setup.py | 40 |
| M | GS018 | dependency_injector_setup.py | 41 |
| M | GS018 | dependency_injector_setup.py | 60 |
| M | GS018 | dependency_injector_setup.py | 61 |
| M | GS018 | dependency_injector_setup.py | 62 |
| M | GS018 | dependency_injector_setup.py | 64 |
| M | GS018 | dependency_injector_setup.py | 65 |
| M | GS018 | dependency_injector_setup.py | 67 |
| M | GS018 | dependency_injector_setup.py | 68 |
| M | GS018 | dependency_injector_setup.py | 69 |
| M | GS018 | dependency_injector_setup.py | 70 |
| M | GS018 | dependency_injector_setup.py | 71 |
| M | GS018 | globals_setup.py | 19 |
| M | GS018 | globals_setup.py | 20 |
| M | GS018 | globals_setup.py | 21 |
| M | GS018 | globals_setup.py | 34 |
| M | GS018 | globals_setup.py | 36 |
| M | GS018 | globals_setup.py | 38 |
| M | GS018 | globals_setup.py | 39 |
| M | GS018 | globals_setup.py | 40 |
| M | GS018 | globals_setup.py | 41 |
| M | GS018 | globals_setup.py | 42 |
| M | GS018 | globals_setup.py | 43 |
| M | GS018 | globals_setup.py | 44 |
| M | GS018 | injector_setup.py | 90 |
| M | GS018 | injector_setup.py | 91 |
| M | GS018 | injector_setup.py | 92 |
| M | GS018 | injector_setup.py | 110 |
| M | GS018 | injector_setup.py | 111 |
| M | GS018 | injector_setup.py | 112 |
| M | GS018 | injector_setup.py | 114 |
| M | GS018 | injector_setup.py | 115 |
| M | GS018 | injector_setup.py | 116 |
| M | GS018 | injector_setup.py | 117 |
| M | GS018 | injector_setup.py | 118 |
| M | GS018 | injector_setup.py | 119 |
| M | GS018 | injector_setup.py | 120 |
| M | GS018 | dishka_setup.py | 27 |
| M | GS018 | dishka_setup.py | 28 |
| M | GS018 | dishka_setup.py | 29 |
| M | GS018 | dishka_setup.py | 48 |
| M | GS018 | dishka_setup.py | 49 |
| M | GS018 | dishka_setup.py | 50 |
| M | GS018 | dishka_setup.py | 52 |
| M | GS018 | dishka_setup.py | 53 |
| M | GS018 | dishka_setup.py | 54 |
| M | GS018 | dishka_setup.py | 55 |
| M | GS018 | dishka_setup.py | 56 |
| M | GS018 | dishka_setup.py | 57 |
| M | GS018 | dishka_setup.py | 58 |
| M | GS018 | that_depends_setup.py | 59 |
| M | GS018 | that_depends_setup.py | 60 |
| M | GS018 | that_depends_setup.py | 61 |
| M | GS018 | that_depends_setup.py | 79 |
| M | GS018 | that_depends_setup.py | 80 |
| M | GS018 | that_depends_setup.py | 81 |
| M | GS018 | that_depends_setup.py | 83 |
| M | GS018 | that_depends_setup.py | 84 |
| M | GS018 | that_depends_setup.py | 85 |
| M | GS018 | that_depends_setup.py | 86 |
| M | GS018 | that_depends_setup.py | 87 |
| M | GS018 | that_depends_setup.py | 88 |
| M | GS018 | that_depends_setup.py | 89 |
| M | GS018 | fastapi_setup.py | 79 |
| M | GS018 | fastapi_setup.py | 80 |
| M | GS018 | fastapi_setup.py | 81 |
| M | GS018 | fastapi_setup.py | 99 |
| M | GS018 | fastapi_setup.py | 100 |
| M | GS018 | fastapi_setup.py | 101 |
| M | GS018 | fastapi_setup.py | 103 |
| M | GS018 | fastapi_setup.py | 104 |
| M | GS018 | fastapi_setup.py | 105 |
| M | GS018 | fastapi_setup.py | 106 |
| M | GS018 | fastapi_setup.py | 107 |
| M | GS018 | fastapi_setup.py | 108 |
| M | GS018 | fastapi_setup.py | 109 |
| M | GS018 | lagom_setup.py | 48 |
| M | GS018 | lagom_setup.py | 49 |
| M | GS018 | lagom_setup.py | 50 |
| M | GS018 | lagom_setup.py | 68 |
| M | GS018 | lagom_setup.py | 69 |
| M | GS018 | lagom_setup.py | 70 |
| M | GS018 | lagom_setup.py | 72 |
| M | GS018 | lagom_setup.py | 73 |
| M | GS018 | lagom_setup.py | 74 |
| M | GS018 | lagom_setup.py | 75 |
| M | GS018 | lagom_setup.py | 76 |
| M | GS018 | lagom_setup.py | 77 |
| M | GS018 | lagom_setup.py | 78 |
| M | GS018 | wireup_setup.py | 30 |
| M | GS018 | wireup_setup.py | 31 |
| M | GS018 | wireup_setup.py | 32 |
| M | GS018 | wireup_setup.py | 50 |
| M | GS018 | wireup_setup.py | 51 |
| M | GS018 | wireup_setup.py | 52 |
| M | GS018 | wireup_setup.py | 54 |
| M | GS018 | wireup_setup.py | 55 |
| M | GS018 | wireup_setup.py | 56 |
| M | GS018 | wireup_setup.py | 57 |
| M | GS018 | wireup_setup.py | 58 |
| M | GS018 | wireup_setup.py | 59 |
| M | GS018 | wireup_setup.py | 60 |
| M | GS018 | diwire_setup.py | 27 |
| M | GS018 | diwire_setup.py | 28 |
| M | GS018 | diwire_setup.py | 29 |
| M | GS018 | diwire_setup.py | 48 |
| M | GS018 | diwire_setup.py | 49 |
| M | GS018 | diwire_setup.py | 50 |
| M | GS018 | diwire_setup.py | 52 |
| M | GS018 | diwire_setup.py | 53 |
| M | GS018 | diwire_setup.py | 54 |
| M | GS018 | diwire_setup.py | 55 |
| M | GS018 | diwire_setup.py | 56 |
| M | GS018 | diwire_setup.py | 57 |
| M | GS018 | diwire_setup.py | 58 |
| M | GS018 | wireup_cbr_setup.py | 20 |
| M | GS018 | wireup_cbr_setup.py | 21 |
| M | GS018 | wireup_cbr_setup.py | 22 |
| M | GS018 | wireup_cbr_setup.py | 44 |
| M | GS018 | wireup_cbr_setup.py | 45 |
| M | GS018 | wireup_cbr_setup.py | 46 |
| M | GS018 | wireup_cbr_setup.py | 48 |
| M | GS018 | wireup_cbr_setup.py | 49 |
| M | GS018 | wireup_cbr_setup.py | 50 |
| M | GS018 | wireup_cbr_setup.py | 51 |
| M | GS018 | wireup_cbr_setup.py | 52 |
| M | GS018 | wireup_cbr_setup.py | 53 |
| M | GS018 | wireup_cbr_setup.py | 54 |
| M | GS018 | routes.py | 22 |
| M | GS018 | handler.py | 18 |
| M | GS018 | bp.py | 32 |
| M | GS018 | bp.py | 33 |
| M | GS018 | router.py | 68 |
| M | GS018 | router.py | 69 |
| M | GS018 | router.py | 71 |
| M | GS018 | router.py | 87 |
| M | GS018 | router.py | 88 |
| M | GS018 | router.py | 118 |
| M | GS018 | router.py | 119 |
| M | GS018 | router.py | 128 |
| M | GS018 | router.py | 129 |
| M | GS018 | cbr.py | 37 |
| M | GS018 | wireup_route.py | 18 |
| M | GS018 | wireup_route.py | 19 |
| M | GS018 | wireup_route.py | 31 |
| M | GS018 | wireup_route.py | 32 |
| M | GS018 | wireup_route.py | 33 |
| M | GS029 | aiohttp.py | 13 |
| C | GS001 | benchmark_results.csv | 2 |
| C | GS001 | benchmark_results.csv | 2 |
| C | GS001 | benchmark_results.csv | 6 |
| C | GS001 | benchmark_results.csv | 8 |
| C | GS001 | benchmark_results.csv | 12 |
| C | GS001 | benchmark_results.csv | 15 |
| C | GS001 | benchmark_results.csv | 17 |
| C | GS001 | benchmark_results.csv | 19 |
| C | GS001 | benchmark_results.csv | 21 |
| C | GS001 | benchmark_results.csv | 23 |
| C | GS001 | benchmark_run_metrics.csv | 17 |
| C | GS001 | benchmark_run_metrics.csv | 61 |
| C | GS001 | benchmark_run_metrics.csv | 72 |
| C | GS001 | benchmark_run_metrics.csv | 81 |
| C | GS001 | benchmark_run_metrics.csv | 89 |
| C | GS001 | benchmark_run_metrics.csv | 100 |
| C | GS001 | benchmark_run_metrics.csv | 108 |
| C | GS001 | benchmark_run_metrics.csv | 109 |
| C | GS001 | benchmark_run_metrics.csv | 120 |
| C | GS001 | benchmark_run_metrics.csv | 122 |
| C | GS001 | benchmark_run_metrics.csv | 126 |
| C | GS001 | benchmark_run_metrics.csv | 133 |
| C | GS001 | benchmark_run_metrics.csv | 141 |
| C | GS001 | benchmark_run_metrics.csv | 145 |
| C | GS001 | benchmark_run_metrics.csv | 148 |
| C | GS001 | benchmark_run_metrics.csv | 150 |
| C | GS001 | benchmark_run_metrics.csv | 157 |
| C | GS001 | benchmark_run_metrics.csv | 161 |
| C | GS001 | benchmark_run_metrics.csv | 165 |
| C | GS001 | benchmark_run_metrics.csv | 168 |
| C | GS001 | benchmark_run_metrics.csv | 169 |
| C | GS001 | benchmark_run_metrics.csv | 181 |
| C | GS001 | benchmark_run_metrics.csv | 198 |
| C | GS001 | benchmark_run_metrics.csv | 206 |
| C | GS001 | benchmark_run_metrics.csv | 213 |
| C | GS001 | benchmark_run_metrics.csv | 217 |
| C | GS001 | benchmark_run_metrics.csv | 229 |
| C | GS001 | benchmark_run_metrics.csv | 237 |
| C | GS001 | benchmark_run_metrics.csv | 240 |
| C | GS001 | benchmark_run_metrics.csv | 261 |
| C | GS001 | benchmark_run_metrics.csv | 263 |
| C | GS001 | benchmark_run_metrics.csv | 264 |
| C | GS001 | benchmark_run_metrics.csv | 272 |
| C | GS001 | benchmark_run_metrics.csv | 281 |
| C | GS001 | benchmark_run_metrics.csv | 289 |
| C | GS001 | benchmark_run_metrics.csv | 296 |
| C | GS001 | benchmark_run_metrics.csv | 296 |
| C | GS001 | benchmark_run_metrics.csv | 301 |
| C | GS001 | benchmark_run_metrics.csv | 305 |
| C | GS001 | benchmark_run_metrics.csv | 312 |
| C | GS001 | benchmark_run_metrics.csv | 325 |
| C | GS001 | benchmark_run_metrics.csv | 329 |
| C | GS001 | benchmark_run_metrics.csv | 340 |
| C | GS001 | benchmark_run_metrics.csv | 344 |
| C | GS001 | benchmark_run_metrics.csv | 349 |
| C | GS001 | benchmark_run_metrics.csv | 353 |
| C | GS001 | benchmark_run_metrics.csv | 357 |
| C | GS001 | benchmark_run_metrics.csv | 360 |
| C | GS001 | benchmark_run_metrics.csv | 361 |
| C | GS001 | benchmark_run_metrics.csv | 377 |
| C | GS001 | benchmark_run_metrics.csv | 377 |
| C | GS001 | benchmark_run_metrics.csv | 384 |
| C | GS001 | benchmark_run_metrics.csv | 397 |
| C | GS001 | benchmark_run_metrics.csv | 405 |
| C | GS001 | benchmark_run_metrics.csv | 408 |
| C | GS001 | benchmark_run_metrics.csv | 421 |
| C | GS001 | benchmark_run_metrics.csv | 425 |
| C | GS001 | benchmark_run_metrics.csv | 425 |
| C | GS001 | benchmark_run_metrics.csv | 445 |
| C | GS001 | benchmark_run_metrics.csv | 453 |
| C | GS001 | benchmark_run_metrics.csv | 457 |
| C | GS001 | benchmark_run_metrics.csv | 468 |
| C | GS001 | benchmark_run_metrics.csv | 473 |
| C | GS001 | benchmark_run_metrics.csv | 480 |
| C | GS001 | benchmark_run_metrics.csv | 481 |
| C | GS001 | benchmark_run_metrics.csv | 488 |
| C | GS001 | benchmark_run_metrics.csv | 492 |
| C | GS001 | benchmark_run_metrics.csv | 493 |
| C | GS001 | benchmark_run_metrics.csv | 501 |
| C | GS001 | benchmark_run_metrics.csv | 517 |
| C | GS001 | benchmark_run_metrics.csv | 526 |
| C | GS001 | benchmark_run_metrics.csv | 537 |
| C | GS001 | benchmark_run_metrics.csv | 539 |
| C | GS001 | benchmark_run_metrics.csv | 545 |
| C | GS001 | benchmark_run_metrics.csv | 554 |
| C | GS001 | benchmark_run_metrics.csv | 560 |
| C | GS001 | benchmark_run_metrics.csv | 565 |
| C | GS001 | benchmark_run_metrics.csv | 566 |
| C | GS001 | benchmark_run_metrics.csv | 569 |
| C | GS001 | benchmark_run_metrics.csv | 577 |
| C | GS001 | benchmark_run_metrics.csv | 589 |
| C | GS001 | benchmark_run_metrics.csv | 593 |
| C | GS001 | benchmark_run_metrics.csv | 593 |
| C | GS001 | benchmark_run_metrics.csv | 600 |
| C | GS001 | benchmark_run_metrics.csv | 601 |
| C | GS001 | benchmark_run_metrics.csv | 612 |
| C | GS001 | benchmark_run_metrics.csv | 613 |
| C | GS001 | benchmark_run_metrics.csv | 621 |
| C | GS001 | benchmark_run_metrics.csv | 632 |
| C | GS001 | benchmark_run_metrics.csv | 637 |
| C | GS001 | benchmark_run_metrics.csv | 661 |
| C | GS001 | benchmark_run_metrics.csv | 665 |
| C | GS001 | benchmark_run_metrics.csv | 669 |
| C | GS001 | benchmark_run_metrics.csv | 684 |
| C | GS001 | benchmark_run_metrics.csv | 689 |
| C | GS001 | benchmark_run_metrics.csv | 689 |
| C | GS001 | benchmark_run_metrics.csv | 697 |
| C | GS001 | benchmark_run_metrics.csv | 709 |
| C | GS001 | benchmark_run_metrics.csv | 713 |
| C | GS001 | benchmark_run_metrics.csv | 733 |
| C | GS001 | benchmark_run_metrics.csv | 734 |
| C | GS001 | benchmark_run_metrics.csv | 737 |
| C | GS001 | benchmark_run_metrics.csv | 740 |
| C | GS001 | benchmark_run_metrics.csv | 757 |
| C | GS001 | benchmark_run_metrics.csv | 761 |
| C | GS001 | benchmark_run_metrics.csv | 793 |
| C | GS001 | benchmark_run_metrics.csv | 800 |
| C | GS001 | benchmark_run_metrics.csv | 805 |
| C | GS001 | benchmark_run_metrics.csv | 828 |
| C | GS001 | benchmark_run_metrics.csv | 829 |
| C | GS001 | benchmark_run_metrics.csv | 833 |
| C | GS001 | benchmark_run_metrics.csv | 842 |
| C | GS001 | benchmark_run_metrics.csv | 852 |
| C | GS001 | benchmark_run_metrics.csv | 853 |
| C | GS001 | benchmark_run_metrics.csv | 857 |
| C | GS001 | benchmark_run_metrics.csv | 861 |
| C | GS001 | benchmark_run_metrics.csv | 862 |
| C | GS001 | benchmark_run_metrics.csv | 877 |
| C | GS001 | benchmark_run_metrics.csv | 888 |
| C | GS001 | benchmark_run_metrics.csv | 900 |
| C | GS001 | benchmark_run_metrics.csv | 905 |
| C | GS001 | benchmark_run_metrics.csv | 909 |
| C | GS001 | benchmark_run_metrics.csv | 910 |
| C | GS001 | benchmark_run_metrics.csv | 913 |
| C | GS001 | benchmark_run_metrics.csv | 920 |
| C | GS001 | benchmark_run_metrics.csv | 925 |
| C | GS001 | benchmark_run_metrics.csv | 927 |
| C | GS001 | benchmark_run_metrics.csv | 929 |
| C | GS001 | benchmark_run_metrics.csv | 933 |
| C | GS001 | benchmark_run_metrics.csv | 944 |
| C | GS001 | benchmark_run_metrics.csv | 956 |
| C | GS001 | benchmark_run_metrics.csv | 977 |
| C | GS001 | benchmark_run_metrics.csv | 986 |
| C | GS001 | benchmark_run_metrics.csv | 997 |
| C | GS001 | benchmark_run_metrics.csv | 998 |
| C | GS001 | benchmark_run_metrics.csv | 1001 |
| C | GS001 | benchmark_run_metrics.csv | 1008 |
| C | GS001 | benchmark_run_metrics.csv | 1009 |
| C | GS001 | benchmark_run_metrics.csv | 1016 |
| C | GS001 | benchmark_run_metrics.csv | 1021 |
| C | GS001 | benchmark_run_metrics.csv | 1025 |
| C | GS001 | benchmark_run_metrics.csv | 1034 |
| C | GS001 | benchmark_run_metrics.csv | 1053 |
| C | GS001 | benchmark_run_metrics.csv | 1080 |
| C | GS001 | benchmark_run_metrics.csv | 1092 |
| C | GS001 | benchmark_run_metrics.csv | 1093 |
| C | GS001 | benchmark_run_metrics.csv | 1106 |
| C | GS001 | benchmark_run_metrics.csv | 1110 |
| C | GS001 | benchmark_run_metrics.csv | 1118 |
| C | GS001 | benchmark_run_metrics.csv | 1121 |
| C | GS001 | benchmark_run_metrics.csv | 1129 |
| C | GS001 | benchmark_run_metrics.csv | 1130 |
| C | GS001 | benchmark_run_metrics.csv | 1141 |
| C | GS001 | benchmark_run_metrics.csv | 1145 |
| C | GS001 | benchmark_run_metrics.csv | 1165 |
| C | GS001 | benchmark_run_metrics.csv | 1173 |
| C | GS001 | benchmark_run_metrics.csv | 1176 |
| C | GS001 | benchmark_run_metrics.csv | 1193 |
| C | GS001 | benchmark_run_metrics.csv | 1201 |
| C | GS001 | pyproject.toml | 79 |
| C | GS001 | pyproject.toml | 86 |
| C | GS001 | pyproject.toml | 87 |
| C | GS001 | pyproject.toml | 95 |
| C | GS001 | pyproject.toml | 108 |
| C | GS001 | pyproject.toml | 110 |
| C | GS001 | pyproject.toml | 145 |
| C | GS001 | pyproject.toml | 154 |
| L | GS003 | bench_runner.py | 115 |
| L | GS003 | bench_runner.py | 117 |
| L | GS003 | bench_runner.py | 119 |
| L | GS003 | bench_runner.py | 125 |
| L | GS003 | bench_runner.py | 127 |
| L | GS003 | bench_runner.py | 129 |
| L | GS003 | bench_runner.py | 342 |
| L | GS003 | bench_runner.py | 389 |
| L | GS003 | bench_runner.py | 396 |
| L | GS003 | bench_runner.py | 466 |
| L | GS003 | bench_runner.py | 470 |
| L | GS003 | bench_runner.py | 472 |
| L | GS003 | bench_runner.py | 482 |
| L | GS003 | bench_runner.py | 483 |
| L | GS003 | bench_runner.py | 485 |
| L | GS003 | bench_runner.py | 486 |
| L | GS003 | bench_runner.py | 674 |
| L | GS003 | bench_runner.py | 689 |
| L | GS003 | bench_runner.py | 691 |
| L | GS003 | bench_runner.py | 693 |
| L | GS003 | generate_charts.py | 115 |
| L | GS003 | generate_charts.py | 128 |
| L | GS003 | generate_tables.py | 273 |
| L | GS003 | generate_tables.py | 312 |
| L | GS003 | generate_tables.py | 315 |
| L | GS003 | generate_versions.py | 56 |
| L | GS003 | generate_versions.py | 74 |
| L | GS008 | bench_runner.py | 78 |
| L | GS008 | types.py | 145 |
| L | GS008 | types.py | 146 |
| I | GS015 | app.py | 11 |
| I | GS015 | app.py | 16 |
| I | GS015 | app.py | 11 |
| I | GS015 | app.py | 16 |
| I | GS015 | app.py | 11 |
| I | GS015 | app.py | 16 |
| I | GS015 | app.py | 7 |
| I | GS015 | asgi.py | 1 |
| i | GS020 |  | 46 |
| H | GS000-LEGACY | bench_runner.py | 71 |
| H | GS000-LEGACY | bench_runner.py | 161 |
| H | GS000-LEGACY | bench_runner.py | 319 |
| C | GS029 | aiohttp.py | 13 |
| H | GS008 | _wrapper_compiler.py | 60 |
| H | GS008 | factory_compiler.py | 281 |
| H | GS004 | _wrapper_compiler.py | 60 |
| H | GS004 | factory_compiler.py | 281 |
| I | GS007 | bench_runner.py | 505 |
| s | GS009 |  | 0 |
| s | GS021 |  | 71 |
| s | GS021 |  | 161 |
| s | GS021 |  | 319 |
| ? | GS025-debug_mode |  | ? |
| ? | GS025-debug_mode |  | ? |
| ? | GS025-debug_mode |  | ? |
| ? | GS025-debug_mode |  | ? |
| ? | GS025-debug_mode |  | ? |
| ? | GS025-debug_mode |  | ? |
| ? | GS025-debug_mode |  | ? |
| ? | GS025-debug_mode |  | ? |
| ? | GS025-debug_mode |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| M | ? | bench_runner.py | 266 |

---
*Сгенерировано GSC v0.6 · 2026-08-08T19:19:24.607064*