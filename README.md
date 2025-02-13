# Bowden Filament Cutter for the Voron Stealthburner


<img width="200" alt="toolhead_CW2" src="https://github.com/user-attachments/assets/51eff1ab-1d54-44e3-b260-746bf7f76ad4" />
<img width="200" alt="toolhead_G2E" src="https://github.com/user-attachments/assets/98eed216-c57a-49ed-b12f-e91e23c47bbf" />
<img width="200" alt="actuator" src="https://github.com/user-attachments/assets/a0ac36f2-673f-483e-953d-081e40a675ca" />

## Introduction
This toolhead integrated filament cutter cuts filament similar to the [filametrix mod](https://github.com/sorted01/Filametrix), on which it is based on, but uses a different approach for actuation by means of an external high torque servo which is connected to the toolhead via a bowden cable.
This way the cutting process is independent of toolhead position/movement and does not introduce any forces to the printer kinematics.

The modification consists of 4 components: a __modified extruder front body__ with bowden cable routing, a __modified printhead__ with shuttle guiding, the __blade shuttle__ and an __external actuator__ which can be clamped to the printer frame extrusions.


## Underlying designs

Because a filament cutter is only useful for multi material printing and multi material printing is very little fun without ECAS and filament sensors the following desings were used as a base instead of the original CW2 or [G2E](https://github.com/JaredC01/Galileo2) parts:

The modified extruder front body for the CW2 is based on [this design](https://www.printables.com/model/466692-stealthburner-cw2-filament-sensors-with-ecas-latch/files) with ECAS and two 5.5mm steelball/microswitch filament sensors

The modified extruder front body for the G2E is based on [this design](https://github.com/juliusjj25/G2E-Filametrix-Lever-Switch-Mod) with ECAS and two DF2-L3-D3 microswitch filament sensors

The printheads are based on the [original voron design printheads](https://vorondesign.com/voron_stealthburner) and the filametrix mod.

## Recent Changes

The original design worked fine, but when cutting harder filaments the required pulling force caused the blade shuttle to tilt when the spring was fully compressed.
Allthough still working this is not nice to look at and also results in unnecessary forces trying to push the extruder to the left and the printhead to the right.
To fix this a limit stop for the blade shuttle has been added to the extruder parts. This limit stop also acts as a "sensor" which closes when the cut is complete.
Also, when cutting hard filament, the wire puller part of the actuator gets damaged (cut by the thin wire) by the thin wire. Therefore reinforcement screws have been added.


---
# Modification Steps
## __Blade Shuttle__
### Required hardware
* 1 [ID 3 x 10 x 3 mm V-Groove Bearing](https://www.amazon.com/Atoplee-3x10x3mm-603VV-Groove-Bearings/dp/B0191I4UU2/ref=sr_1_3?crid=144OG5RS855RQ&dib=eyJ2IjoiMSJ9.mrEt9I1UqIiOuWrEH5YhCtw7eSiIj3BJY1ERlS7qMZYBm4F7BR77bywRA2RKzA6pOuv-iEsmjQ0ztewyvq1LfbGmRYdDwDGrlDRlKRygTiJ5LppiQeL3T_C6_7eR0gzQabn-PX2flqK8z4l_D-ABezJ0InUYtu96bgfy8sgNW2So3pft-zeVH6scui8fGYFbJ32vOz6YZVLCzRxXSQY6oLToennecodWFsqMVICKwuI.jYywOA16bapkbsYEVzsdyqeZvgXNYHbvygkg1QdUzIk&dib_tag=se&keywords=bearing+3x10x3+v+groove&qid=1738349937&sprefix=bearing+3x10x3+v+groov%2Caps%2C174&sr=8-3)
* 1 M2.5 x 8 countersunk head screw  -OR-  M2.5 x 8 screw + Brass tube OD 3 mm / ID 2.5 mm, L 3 mm 
* 1 M2.5 washer
* 1 M2.5 x 5 x 3.5 heat set insert ([from this sortiment](https://www.amazon.com/Threaded-Inserts-Assortment-Printing-Injection/dp/B0D49Y8J6M/ref=sr_1_32_sspa?crid=37N9WY18Y1Q59&dib=eyJ2IjoiMSJ9.IhC2XS8BWkmBeVWTnCF6LHlI6bbjIridYa900Ri9OL1xQQVtByy2Pq8GWeAglwM_ijbtKla2l07NH8vg2BESD1hA89qBw4X6IWKskARlL6zzCi0_OifI62FObqPf7ACnprQaeRiOTLDV5DMxxyXPfGPRIG4DHwIQeGXHi3N76v3tmVqy3i_n2O9OqzDZtH9r.kcEL0XpSwtg5Td_4TtDF3OsBxWow7K60BTEkWebAI9Q&dib_tag=se&keywords=M2.5+x+5+x+3.5&qid=1738014336&sprefix=m2.5+x+5+x+3.5%2Caps%2C324&sr=8-32-spons&xpid=_lenikuANp8ye&sp_csd=d2lkZ2V0TmFtZT1zcF9idGY&psc=1))
* 1 compression spring 5.5 x 17 mm ([from this sortiment](https://www.amazon.com/dp/B0DF21GRN1/ref=sr_1_1_sspa?__mk_de_DE=ÅMÅŽÕÑ&crid=2AKV6FXLFZY04&dib=eyJ2IjoiMSJ9.B9q0atkenJRq4xFEpuA6kf0xvpWVwtjE_6Jrg8n_wl6NHta9ITOqniu6mMLtZMFY2_GtR4F_p8Hx75KQDkPY7fpfaDna87tC5B3B3hsjJfN4gQ8lqOv1fjgLgXU953trXPpknKVWs0QRSiNBvWAiD5JjdxLaEr9TSl6Sqnwv4ecXGIxPsb15RojaRq2vxIcHnsdGiSbCrEg-Z74QEsWqzqf3JAr6EFOmu-LbFnp-Fyk.SwDMcXsodjg3r6qEAGHaBXy8vgAhajbzSszQWizHb5c&dib_tag=se&keywords=compression+spring&qid=1736647255&sprefix=compression+spring%2Caps%2C199&sr=8-1-spons&sp_csd=d2lkZ2V0TmFtZT1zcF9hdGY&psc=1))
* 1 [Hobby knife blade # 4](https://www.amazon.com/CIMAXIC-Manganese-Carving-Replacement-Supplies/dp/B0DJX43D77/ref=sr_1_112?crid=2D6MJ2VXDM7MM&dib=eyJ2IjoiMSJ9.LY9KWgul7GfhchyOrpz6t1ZtBqw-xa3UTVVfifRutwFS_irrVL1G9lXfELgCCHIU7v4Vs4RGDzlct3djc7pDxj04-_vz_afMDG0CRPNhCx9S9MKe8RPKbRVZ4hAVBwq2QfyRmpew2Zg8lfiFboFDnUSKugyBYasF7VfptCyb8PoF0xozSM4wEwvciMsC-kEJ3F7XI1KiUO2xdIGADbwYVwU0KrWm6srWC1qPjIQd-GFrRmOWRcXC0eaKomWlNA5ueOJzOzIh-PyYU6ZmuL2snytGIipbJ51XFjx65Ti0iDtjue3wFclblNAQJQXi3BaG2lXQBZqatxCImovVcprdC0yudAjnQ6Mx2bZvxthwV-ia6OJdKMpNR-Wn9GSo3RDzTp6Vb38nd8af7AWgnc04BREyjz2SfUPNtj9Mu_UtjY6tioOZq7D_8-a8DNVGuDvy.SGOFwUSK3z_uNxu1zXh5N-71SdCpIgs06duCPREJyNc&dib_tag=se&keywords=hobby+knife+blade+%234&qid=1738016804&sprefix=hobby+knife+blade+4%2Caps%2C215&sr=8-112&xpid=7l1eXVoBFqf5t) (cut or broken off at the end of the slot)
### Printed parts
| Picture | Description | STL | STEP |
| :---: | :---: | :---: | :---: |
| <img width="100" alt="Shuttle" src="https://github.com/user-attachments/assets/807fdf26-4689-4989-b387-cf6e7b295a66" /> | Blade shuttle  | [stl](https://github.com/weuzor/bowden_cutter/blob/main/STL/Blade%20Shuttle%20Parts/Shuttle.stl) | [step](https://github.com/weuzor/bowden_cutter/blob/main/CAD/Blade%20Shuttle%20Parts/Shuttle.step) |
### Assembly
* Break off the blade #4 near the end of the slot
* Install the heat set insert in the printed part 
* Assemble as shown.
  Note: Unfortunately the blade slot width is too small for a M3 screw to fit through, so M2.5 it has to be. However, the pulley inner diameter is 3 mm. In order to keep the pulley centered either use something like a brass tube OD 3 mm / ID 2.5 mm, L 3 mm or some heatshrink over the last 3 mm of the screw thread.
Altertnatively, a well tightened countersunk head screw can also be used.
<img width="200" alt="Blade Shuttle Assembly Option 1" src="https://github.com/user-attachments/assets/db6b5380-9cc0-4790-899d-9d4d9be7db8c" />
<img width="200" alt="Blade Shuttle Assembly Option 2" src="https://github.com/user-attachments/assets/238e395d-fdba-479d-b0bf-4a419ff798be" />
<img width="200" alt="blade_shuttle_and_spring" src="https://github.com/user-attachments/assets/ffe18d68-5cea-42b8-bd15-451c5dcee94c" />


---
## Extruder 
### Required hardware
* PTFE tube 2mm/4mm ([amazon](https://www.amazon.com/Quickun-Teflon-Tubing-Printer-Length/dp/B08Q813BQV/ref=sr_1_3?crid=1R3J14UI2HSSZ&dib=eyJ2IjoiMSJ9.S_VpxsGc1zg6aRWr3AxoeBAf3HmhriQkxaPrURjIm19fUNdgjOuSV88yyRDn13jfGc-KFowX_gQBx3KJlyErb16wcQiwJOANSmfdUXMBtQMD5dOMtogpyb2nECOL0kZt6lXGe3abvwchYJEQ1fJlvJvXZIlnFkGkY4cCw4A2V1gnN0ct6xzFrNsVg1pD8BiY4BJd8zQe8kqLLALJZUWfRX78Lp720qSnAV27_03j8Nk.B13xI1TJrRLbN7JsXPVuJVxegMIvsJkswggzAE3v7W8&dib_tag=se&keywords=ptfe%2Btube%2B1mm%2B%2F%2B2mm&qid=1738015104&sprefix=ptfe%2Btube%2B1mm%2B%2F%2B2mm%2Caps%2C167&sr=8-3&th=1))
* PTFE Tube 1mm/2mm ([amazon](https://www.amazon.com/Quickun-Teflon-Tubing-Printer-Length/dp/B08Q83XNTT/ref=sr_1_3?crid=1R3J14UI2HSSZ&dib=eyJ2IjoiMSJ9.S_VpxsGc1zg6aRWr3AxoeBAf3HmhriQkxaPrURjIm19fUNdgjOuSV88yyRDn13jfGc-KFowX_gQBx3KJlyErb16wcQiwJOANSmfdUXMBtQMD5dOMtogpyb2nECOL0kZt6lXGe3abvwchYJEQ1fJlvJvXZIlnFkGkY4cCw4A2V1gnN0ct6xzFrNsVg1pD8BiY4BJd8zQe8kqLLALJZUWfRX78Lp720qSnAV27_03j8Nk.B13xI1TJrRLbN7JsXPVuJVxegMIvsJkswggzAE3v7W8&dib_tag=se&keywords=ptfe%2Btube%2B1mm%2B%2F%2B2mm&qid=1738015104&sprefix=ptfe%2Btube%2B1mm%2B%2F%2B2mm%2Caps%2C167&sr=8-3&th=1))
* Nylon coated stranded steel wire 0.6 mm diameter ([amazon](https://www.amazon.com/BENECREAT-120-Feet-0-024inch-7-Strand-Stainless/dp/B07V3S947N/ref=sr_1_1?crid=1BYTPFOE6298L&dib=eyJ2IjoiMSJ9.pXWOElTDcRCUMASCv9CG5wXzqwG73bFkvewBUseXkb4tqkT_feMtAnXleQMdtJwa1oJMVtIszDzXwfPblYfP64tjXdP9F0iR_1J98SfKH-j3-fo3k9ePpBVRJ0csdYJa9CZaTuUSf8O_wQcU24RNqQAZuUvfDrIYvizzCy__HNGWRK7X2O2HsMPVSKmtDl2pop2ThvJM-srOzA1oyOzmC4VnYbJhEU7rtQzXOn9QE80v0H_KpDV_ERNIVkvUmvCNSLtCG5sN_CnxIvamUS2CC-3Q7Xl_GcmsOA9o3AAR-lJFj4jYSLso0E3xXZg1NsyL5WdYJ2gr_x8npbPRsDBxN2HjJLR8NSTjabgi2uYDfdlkFbYhq287YNxPa0I8yPV1dDAeuAxmDDJxgkyBQxIXYs7bOJ3_x4oeutiirFGdfPy9Q2FBzmaN8RU3tMkjiLn7.D-khznNCXsM-Zj6h4FykYFTd3pSIbRoA7DrW9yir5Nc&dib_tag=se&keywords=steel%2Bwire%2B0.6%2Bmm%2Bbenecreat&qid=1736648346&sprefix=steel%2Bwire%2B0.6%2Bmm%2Bbenecreat%2Caps%2C184&sr=8-1&th=1))
* 2 M1.6 x 3 Screws
### Printed parts
#### Galileo 2
| Picture | Description | STL | STEP |
| :---: | :---: | :---: | :---: |
| <img width="200" alt="G2E_Front_Body" src="https://github.com/user-attachments/assets/b586abdd-91f1-4f26-bc0d-28a4453b21db" /> | G2E Front Body with two ball less filament sensors, bowden tube routing, ECAS, cutter endstop | [stl](https://github.com/weuzor/bowden_cutter/blob/main/STL/Extruder%20Parts/G2E/G2E_Front_Body.stl) | [step](https://github.com/weuzor/bowden_cutter/blob/main/CAD/Extruder%20Parts/G2E/G2E_Front_Body.step) | 
#### Clockwork 2
| Picture | Description | STL | STEP |
| :---: | :---: | :---: | :---: |
| <img width="200" alt="CW2 Front Body (new)" src="https://github.com/user-attachments/assets/01b24885-97a2-4376-a4f6-a0f549d33356" /> | CW2 Front Body (new motor plate) with two filament sensors, bowden tube routing, ECAS, cutter endstop | [stl](https://github.com/weuzor/bowden_cutter/blob/main/STL/Extruder%20Parts/CW2/CW2_Front_Body_new_motorplate.stl) | [step](https://github.com/weuzor/bowden_cutter/blob/main/CAD/Extruder%20Parts/CW2/CW2_Front_Body_new_motorplate.step) |
| <img width="200" alt="CW2 Front Body (old)" src="https://github.com/user-attachments/assets/0be7a897-4f9f-4f70-8ebc-cd91dcf4e384" /> | Same as above but compatible with the old motor plate | [stl](https://github.com/weuzor/bowden_cutter/blob/main/STL/Extruder%20Parts/CW2/CW2_Front_Body_old_motorplate.stl) | [step](https://github.com/weuzor/bowden_cutter/blob/main/CAD/Extruder%20Parts/CW2/CW2_Front_Body_old_motorplate.step) |
### Assembly
* Cut the 2mm/4mm PTFE tube to the required length for the installation (depending on printer size and where the actuator will be located).
* Cut the 1mm/2mm PTFE tube approximately 10 cm longer than the 2mm/4mm tube
* Tie a [figure-8-knot](https://www.animatedknots.com/figure-8-knot) in the 0.6 mm wire and cut it approximately 10 cm longer than the 1mm/2mm PTFE tube (measured from the knot)
* Check that the OD 4 mm PTFE fits into its recess on top of the printed body. Clear out by hand with a 4mm drill if necessary.
* Check that the 0.6 mm wire can be inserted in the small holes at the bottom aof the printed body. Clear out by hand with a 1 mm drill if necessary.
* Push the OD 2 mm PTFE from the top into the printed body until it is fully inserted. Might need a bit of persuasion here and there but is definitely doable. A drop of oil and a 2 steps forward one step back movement strategy helps. If you can insert the 0.6 mm wire from the opposite side without catching the on the PTFE tube edge you are there.
* Slide the ID 2mm OD 4mm PTFE over the ID 1 mm OD 2mm PTFE tube and push firmly into its recess in the printed part.
* Cut the inner PTFE tube flush with the outer tube
* Push the 0.6 mm wire through the long hole at the bottom of the printed part and pull firmly to fully tighten the knot. Clip off the excess wire leaving about 1 mm.
* After a U-turn push the wire through the PTFE until it comes out the other end
* Complete the extruder with the modified body part
<img width="300" alt="bowden_installation_cw2" src="https://github.com/user-attachments/assets/132a8e65-78a3-4f40-8ac7-77b1851f4673" />
<img width="300" alt="bowden_installation_g2e" src="https://github.com/user-attachments/assets/daf4e99b-cb09-4b16-b12f-eaf5a2dc0a12" />
<img width="300" alt="cut_sensor_inst" src="https://github.com/user-attachments/assets/d13eb39e-dd16-4df5-88e7-a9adbdb015e4" />
<img width="300" alt="cut_sensor" src="https://github.com/user-attachments/assets/3debba23-c78c-47de-ba56-253c560cbdb4" />


---
## Printhead
### Required hardware
* 1 M3 Nut
* Filament path PTFE Tube
### Printed parts
#### E-RV
| Picture | Description | STL | STEP |
| :---: | :---: | :---: | :---: |
| <img width="100" alt="E-RV (no ADXL)_Front" src="https://github.com/user-attachments/assets/f26e07c7-f908-46e2-90c3-319bb0e2d7c8" /> <img width="100" alt="E-RV (no ADXL)_Back" src="https://github.com/user-attachments/assets/885e5c1f-8065-4ccf-b9a9-b7af91be8f2e" /> | E-RV Printhead (symmetric, no ADXL mount) with blade shuttle guiding | [front](https://github.com/weuzor/bowden_cutter/blob/main/STL/Printhead%20Parts/E-RV/E-RV%20(no%20ADXL)_Front.stl) [back](https://github.com/weuzor/bowden_cutter/blob/main/STL/Printhead%20Parts/E-RV/E-RV%20(no%20ADXL)_Back.stl) | [front](https://github.com/weuzor/bowden_cutter/blob/main/CAD/Printhead%20Parts/E-RV/E-RV%20(no%20ADXL)_Front.step) [back](https://github.com/weuzor/bowden_cutter/blob/main/CAD/Printhead%20Parts/E-RV/E-RV%20(no%20ADXL)_Back.step) |
| <img width="100" alt="E-RV_Front" src="https://github.com/user-attachments/assets/5078bad3-698e-4179-b9c1-45ca5a2eb1b4" /> <img width="100" alt="E-RV_Back" src="https://github.com/user-attachments/assets/9fa90508-897d-4265-bfb4-c5f339c0262c" /> | Stock E-RV printhead with blade shuttle linear guiding  | [front](https://github.com/weuzor/bowden_cutter/blob/main/STL/Printhead%20Parts/E-RV/E-RV_Front.stl) [back](https://github.com/weuzor/bowden_cutter/blob/main/STL/Printhead%20Parts/E-RV/E-RV_Back.stl) | [front](https://github.com/weuzor/bowden_cutter/blob/main/CAD/Printhead%20Parts/E-RV/E-RV_Front.step) [back](https://github.com/weuzor/bowden_cutter/blob/main/CAD/Printhead%20Parts/E-RV/E-RV_Back.step) |
#### P-RPDV2
| Picture | Description | STL | STEP |
| :---: | :---: | :---: | :---: |
| <img width="100" alt="P-RPDV2_Front" src="https://github.com/user-attachments/assets/12312cef-ea5a-4f57-8c93-62cf0aa668e6" /> <img width="100" alt="P-RPDV2_Back" src="https://github.com/user-attachments/assets/5e2eb361-e8f2-40f8-964a-880e0bdca1bf" /> | Stock P-RPDV2 printhead with blade shuttle linear guiding  | [front](https://github.com/weuzor/bowden_cutter/blob/main/STL/Printhead%20Parts/P-RPDV2/P-RPDV2_Front.stl) [back](https://github.com/weuzor/bowden_cutter/blob/main/STL/Printhead%20Parts/P-RPDV2/P-RPDV2_Back.stl) | [front](https://github.com/weuzor/bowden_cutter/blob/main/CAD/Printhead%20Parts/P-RPDV2/P-RPDV2_Front.step) [back](https://github.com/weuzor/bowden_cutter/blob/main/CAD/Printhead%20Parts/P-RPDV2/P-RPDV2_Back.step) |
#### P-DRG
| Picture | Description | STL | STEP |
| :---: | :---: | :---: | :---: |
| <img width="100" alt="P-DRG_Front" src="https://github.com/user-attachments/assets/900afa84-4165-4a2c-becd-abb6d53780e5" /> <img width="100" alt="P-DRG_Back" src="https://github.com/user-attachments/assets/e7910e98-b0cc-4afe-924f-38e42218f14a" /> | Stock P-DRG printhead with blade shuttle linear guiding  | [front](https://github.com/weuzor/bowden_cutter/blob/main/STL/Printhead%20Parts/P-DRG/P-DRG_Front.stl) [back](https://github.com/weuzor/bowden_cutter/blob/main/STL/Printhead%20Parts/P-DRG/P-DRG_Back.stl) | [front](https://github.com/weuzor/bowden_cutter/blob/main/CAD/Printhead%20Parts/P-DRG/P-DRG_Front.step) [back](https://github.com/weuzor/bowden_cutter/blob/main/CAD/Printhead%20Parts/P-DRG/P-DRG_Back.step) |
### Assembly

*  Assemble as usual. Don't forget the ptfe tube before inserting the M3 nut
*  Check that the spring followed by the blade shuttle can be inserted into the guide and moves smoothly
*  Optionally lubricate the contact surfaces with a tiny amount of petroleum jelly
*  Remove blade shuttle and spring for now


<img width="200" alt="shuttle_insert" src="https://github.com/user-attachments/assets/2a024b0f-e332-44d9-b8a5-d60f1ee4a10f" />
<img width="200" alt="shuttle_inserted" src="https://github.com/user-attachments/assets/743af695-8908-4491-90c2-b63257692f08" />
<img width="200" alt="shuttle_cut_pos" src="https://github.com/user-attachments/assets/c7732227-5de3-47bd-b79d-d00c3ea9141c" />


---

## Actuator

### Required hardware
* 1 [Miuzei 25kg Servo](https://www.amazon.com/Miuzei-Waterproof-Compatible-Steering-Horn（270°）/dp/B0C5LTKBD4/ref=sr_1_8?crid=1RKYBOP2MC3X5&dib=eyJ2IjoiMSJ9.5BsLf39L1mf4c0ZP7ihNfBcTucSXzqrylZ5wPm1FCZv5wywgXEZg8dzhwaeOFhQKoNJWUU3jyFHMdI_3LbyACR33Kmu10v0dFclbm8f5Wi29QDhH9nP2OV--_QzTVKYJtExh0ru4tfxeGZCQR1O45u62ZbZ7vDu3kLlgaTb16AaTpBTvtNuceMTKtBs_AoUUucpRz8daa88bTl0jgQc3zPhm-HagKRoHf3OntGky96HSfhzFnBvgk_47v8lISK_yfMscdNapOXOrRZh-QcGOnMjBkn3Q2Z7BgruQQfZQg2Dosnl2Lo9nXBHNfwN3vcMU5GP0gaHs4a_NLZ4IQaibOTazYqvwFS1RVYBUXIoopTEp9_zGB0G0D4ItZ_uS9RlO99e3KistSzl-Ztef1v2GcOVwoBLVwRXQxPFw_HdreqIyc5iuHV7sSS0DYl1A8Qrn._j4nZ8dHQSZ3S-M3PkTiq-Yw1uM0tN85bQJuZTc3dog&dib_tag=se&keywords=miuzei&qid=1738536290&sprefix=miuzei%2Caps%2C181&sr=8-8&th=1) (or similar) + supplied screws + round servo horn
* 2 M3 x 4 x 5 heat set inserts
* 2 M3 washer
* 2 M3 x 5 screws
* 4 M2 x 8 Tapping screws
* 1 ECAS Collet (rubber part removed)
### Printed parts
| Picture | Description | STL | STEP |
| :---: | :---: | :---: | :---: |
| <img width="100" alt="Servo_Frame_Mount" src="https://github.com/user-attachments/assets/0e193ddf-345c-4ca8-8349-a6c4eaba5648" /> | Actuator servo to frame mount | [stl](https://github.com/weuzor/bowden_cutter/blob/main/STL/Actuator%20Parts/Servo_Frame_Mount.stl) | [step](https://github.com/weuzor/bowden_cutter/blob/main/CAD/Actuator%20Parts/Servo_Frame_Mount.step) |
| <img width="100" alt="Servo_Frame_Mount_Mirrored" src="https://github.com/user-attachments/assets/6a947454-1792-4077-9af6-5da123a04a85" /> | Actuator servo to frame mount, mirrored   | [stl](https://github.com/weuzor/bowden_cutter/blob/main/STL/Actuator%20Parts/Servo_Frame_Mount_mirrored.stl) | [step](https://github.com/weuzor/bowden_cutter/blob/main/CAD/Actuator%20Parts/Servo_Frame_Mount_mirrored.step) |
| <img width="100" alt="Servo_Frame_Mount_Clamp_Insert" src="https://github.com/user-attachments/assets/c4f4a299-49c2-4280-9b61-5a2158216f7c" /> | clamp insert ( x2 ) | [stl](https://github.com/weuzor/bowden_cutter/blob/main/STL/Actuator%20Parts/Servo_Frame_Mount_Clamp_Insert_x2.stl) | [step](https://github.com/weuzor/bowden_cutter/blob/main/CAD/Actuator%20Parts/Servo_Frame_Mount_Clamp_Insert_x2.step) |
| <img width="100" alt="Wire_Puller" src="https://github.com/user-attachments/assets/b636efdd-fa4a-4a45-bc94-c9c16d2ef66e" /> | wire puller servo attachment| [stl](https://github.com/weuzor/bowden_cutter/blob/main/STL/Actuator%20Parts/Wire_Puller.stl) | [step](https://github.com/weuzor/bowden_cutter/blob/main/CAD/Actuator%20Parts/Wire_Puller.step) |
### Assembly
* Press the ECAS collet and two clamp inserts into the servo mount body as shown
* Install the two heat set inserts in the wire puller part and assemble as shown with the round servo horn which comes with the servo.
* Combine everything as shown
<img width="200" alt="actuator_body" src="https://github.com/user-attachments/assets/d5922760-ac2b-4eee-b079-ff1ca9ba5038" />
<img width="200" alt="actuator_puller" src="https://github.com/user-attachments/assets/54071c3e-76d2-4f79-a27c-11835c298704" />
<img width="200" alt="actuator_servoy" src="https://github.com/user-attachments/assets/6603d521-6a93-4eaa-b773-dcf1c5fdcd0b" />

## FINAL STEPS
<img width="200" alt="actuator_wire" src="https://github.com/user-attachments/assets/285d378b-fa9a-4ebf-b4ba-dc3898706fe0" />
<img width="200" alt="shuttle_pos" src="https://github.com/user-attachments/assets/45f206ec-e55d-49cf-a1fb-1d73ee3a89b3" />

* Assemble the toolhead with the modified extruder and printhead
* Run the bowden wire through the actuator hole and insert the ptfe tubes into the ecas collet
* Insert the blade shuttle and place the wire loop around the pulley
* Loosen the wire clamp bolts and route the wire on the actuator servo as shown
* Adjust the wire length so that the blade shuttle is flush with the printhead edge and the servo is approximately in the shown position (servo angle 90 deg)
* Tighten the wire clamp bolts



