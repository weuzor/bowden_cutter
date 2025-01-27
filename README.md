# Bowden Filament Cutter for Voron Stealthburner



With the following modifications the Voron Stealthburner will be able to cut filament independent of toolhead position and and without generating any forces to the xy belts.
The price to pay is a second PTFE tube coming out of the printhead which is more or less permanently attached to the bowden actuator.

<img width="438" alt="toolhead_CW2" src="https://github.com/user-attachments/assets/51eff1ab-1d54-44e3-b260-746bf7f76ad4" />
<img width="438" alt="toolhead_G2E" src="https://github.com/user-attachments/assets/98eed216-c57a-49ed-b12f-e91e23c47bbf" />

---

## BLADE SHUTTLE
### Required hardware
* 1 M2.5 x 8 screw +  Brass tube OD 3 mm / ID 2.5 mm, L 3 mm OR  1 M2.5 x 8 screw with heat shrink tube over the last 3 mm of the thread OR 1 M2.5 x 8 countersunk head screw
* 1 M2.5 washer
* 1 M2.5 x 5 x 3.5 heat set insert
* 1 compression spring 5.5 x 17 mm ([from this sortiment](https://www.amazon.com/dp/B0DF21GRN1/ref=sr_1_1_sspa?__mk_de_DE=ÅMÅŽÕÑ&crid=2AKV6FXLFZY04&dib=eyJ2IjoiMSJ9.B9q0atkenJRq4xFEpuA6kf0xvpWVwtjE_6Jrg8n_wl6NHta9ITOqniu6mMLtZMFY2_GtR4F_p8Hx75KQDkPY7fpfaDna87tC5B3B3hsjJfN4gQ8lqOv1fjgLgXU953trXPpknKVWs0QRSiNBvWAiD5JjdxLaEr9TSl6Sqnwv4ecXGIxPsb15RojaRq2vxIcHnsdGiSbCrEg-Z74QEsWqzqf3JAr6EFOmu-LbFnp-Fyk.SwDMcXsodjg3r6qEAGHaBXy8vgAhajbzSszQWizHb5c&dib_tag=se&keywords=compression+spring&qid=1736647255&sprefix=compression+spring%2Caps%2C199&sr=8-1-spons&sp_csd=d2lkZ2V0TmFtZT1zcF9hdGY&psc=1)
* 1 Hobby knife blade # 4 (cut or broken off at the end of the slot)
### Printed parts
| Picture | Description | STL | STEP |
| :---: | :---: | :---: | :---: |
| <img width="100" alt="Shuttle" src="https://github.com/user-attachments/assets/807fdf26-4689-4989-b387-cf6e7b295a66" /> | Blade shuttle  | [stl](https://github.com/weuzor/bowden_cutter/blob/main/STL/Blade%20Shuttle%20Parts/Shuttle.stl) | [step](https://github.com/weuzor/bowden_cutter/blob/main/CAD/Blade%20Shuttle%20Parts/Shuttle.step) |
### Assembly
* Break off the blade #4 near the end of the slot
* Install the heat set insert in the printed part 
* Assemble as shown. 
Unfortunately the blade slot width is too small for a M3 screw to fit through, so M2.5 it must be.
However, the pulley inner diameter is 3 mm. In order to keep the pulley centered either use something like a Brass tube OD 3 mm / ID 2.5 mm, L 3 mm or some heatshrink over the last 3 mm of the srew thread.
Altertnatively, a well tightened countersunk head screw can also be used.
<img width="300" alt="Blade Shuttle Assembly Option 1" src="https://github.com/user-attachments/assets/db6b5380-9cc0-4790-899d-9d4d9be7db8c" />
<img width="300" alt="Blade Shuttle Assembly Option 2" src="https://github.com/user-attachments/assets/238e395d-fdba-479d-b0bf-4a419ff798be" />

---
## EXTRUDER
### Required hardware
* PTFE tube 2mm/4mm
* PTFE Tube 1mm/2mm
* Nylon coated stranded steel wire 0.6 mm diameter ([amazon](https://www.amazon.com/BENECREAT-120-Feet-0-024inch-7-Strand-Stainless/dp/B07V3S947N/ref=sr_1_1?crid=1BYTPFOE6298L&dib=eyJ2IjoiMSJ9.pXWOElTDcRCUMASCv9CG5wXzqwG73bFkvewBUseXkb4tqkT_feMtAnXleQMdtJwa1oJMVtIszDzXwfPblYfP64tjXdP9F0iR_1J98SfKH-j3-fo3k9ePpBVRJ0csdYJa9CZaTuUSf8O_wQcU24RNqQAZuUvfDrIYvizzCy__HNGWRK7X2O2HsMPVSKmtDl2pop2ThvJM-srOzA1oyOzmC4VnYbJhEU7rtQzXOn9QE80v0H_KpDV_ERNIVkvUmvCNSLtCG5sN_CnxIvamUS2CC-3Q7Xl_GcmsOA9o3AAR-lJFj4jYSLso0E3xXZg1NsyL5WdYJ2gr_x8npbPRsDBxN2HjJLR8NSTjabgi2uYDfdlkFbYhq287YNxPa0I8yPV1dDAeuAxmDDJxgkyBQxIXYs7bOJ3_x4oeutiirFGdfPy9Q2FBzmaN8RU3tMkjiLn7.D-khznNCXsM-Zj6h4FykYFTd3pSIbRoA7DrW9yir5Nc&dib_tag=se&keywords=steel%2Bwire%2B0.6%2Bmm%2Bbenecreat&qid=1736648346&sprefix=steel%2Bwire%2B0.6%2Bmm%2Bbenecreat%2Caps%2C184&sr=8-1&th=1))
### Printed parts
#### Galileo 2
| Picture | Description | STL | STEP |
| :---: | :---: | :---: | :---: |
| <img width="100" alt="G2E_Front_Body" src="https://github.com/user-attachments/assets/37f58180-d7a9-494c-8c6e-711cfa0e8764" /> | G2E Front Body with two ball less filament sensors and bowden tube routing | [stl](https://github.com/weuzor/bowden_cutter/blob/main/STL/Extruder%20Parts/G2E/G2E%20Front%20Body%20with%20bowden%20cutter%2C%20ECAS%20and%20sensors.stl) | [step](https://github.com/weuzor/bowden_cutter/blob/main/CAD/Extruder%20Parts/G2E/G2E%20Front%20Body%20with%20bowden%20cutter%2C%20ECAS%20and%20sensors.step) | 
#### Clockwork 2
| Picture | Description | STL | STEP |
| :---: | :---: | :---: | :---: |
| <img width="100" alt="CW2 Front Body (new)" src="https://github.com/user-attachments/assets/6d4e50ab-400f-4ecb-8292-1e488efb2b5d" /> | CW2 Front Body with ECAS, two 5.5 mm steel ball / D2F filament sensors and bowden cutter tube routing. Compatible with the new motor plate | [stl](https://github.com/weuzor/bowden_cutter/blob/main/STL/Extruder%20Parts/CW2/CW2%20Front%20Body%20with%20bowden%20cutter%2C%20ECAS%20and%20sensors%20(new).stl) | [step](https://github.com/weuzor/bowden_cutter/blob/main/CAD/Extruder%20Parts/CW2/CW2%20Front%20Body%20with%20bowden%20cutter%2C%20ECAS%20and%20sensors%20(new).step) |
| <img width="100" alt="CW2 Front Body (old)" src="https://github.com/user-attachments/assets/33276c96-8997-4511-af02-54d02b0d76e8" /> | Same as above but compatible with the old motor plate | [stl](https://github.com/weuzor/bowden_cutter/blob/main/STL/Extruder%20Parts/CW2/CW2%20Front%20Body%20with%20bowden%20cutter%2C%20ECAS%20and%20sensors%20(old).stl) | [step](https://github.com/weuzor/bowden_cutter/blob/main/CAD/Extruder%20Parts/CW2/CW2%20Front%20Body%20with%20bowden%20cutter%2C%20ECAS%20and%20sensors%20(old).step) |
### Assembly
* Cut the 2mm/4mm PTFE tube to the required length for the installation (depending on printer size and where the actuator will be located).
* Cut the 1mm/2mm PTFE tube approximately 10 cm longer than the 2mm/4mm tube
* Tie a [figure-8-knot](https://www.animatedknots.com/figure-8-knot) in the 0.6 mm wire and cut it approximately 10 cm longer than the 1mm/2mm PTFE tube (measured from the knot)
* Check that the OD 4 mm PTFE fits into its recess on top of the printed body. Clear out by hand with a 4mm drill if necessary.
* Check that the 0.6 mm wire can be inserted in the small holes at the bottom aof the printed body. Clear out by hand with a 1 mm drill if necessary.
* Push the OD 2 mm PTFE from the top into the printed body until it is fully inserted. Might need a bit of persuasion here and there but is definitely doable. A drop of oil and a 2 steps forward one step back movement strategy helps. If you can insert the 0.6 mm wire from the opposite side without catching the on the PTFE tube edge you are there.
* Slide the ID 2mm OD 4mm PTFE over the ID 1 mm OD 2mm PTFE tube and push firmly into its recess in the prited part.
* Cut the inner PTFE tube flush with the outer tube
* Push the 0.6 mm through the long hole at the bottom of the printed part and pull firmly to fully tighten the knot. Clip off the excess wire leaving about 1 mm.
* After a U-turn push the wire through the PTFE until it comes out the other end
<img width="500" alt="bowden_installation_cw2" src="https://github.com/user-attachments/assets/132a8e65-78a3-4f40-8ac7-77b1851f4673" />
<img width="500" alt="bowden_installation_g2e" src="https://github.com/user-attachments/assets/daf4e99b-cb09-4b16-b12f-eaf5a2dc0a12" />

---
## PRINTHEAD
### Required hardware
* 1 M3 Nut
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

Assemble as usual insert the spring and the blade shuttle. Lubricate with a tiny amount of petroleum jelly.

---

## ACTUATOR

### Required hardware
* 1 [Miuzei 25kg Servo](https://www.amazon.com/Miuzei-Waterproof-Compatible-Steering-Horn（270°）/dp/B0C5LWHTQ1/ref=sr_1_5?crid=254V5NK70U1TP&dib=eyJ2IjoiMSJ9.xl7ViI1L6GDxIebmAsDF61VWxHk4vy3dKQsGj3yWRiow6rIHsWr-hCJJq2MChSZdLm2EW8oyL1CGCbhzLVqA37xbgqk7q_-EQPKaeXZnQrtgoqqqCbxr0edXhiQ99DqLxOY53BRdwveFjd_xQ7G-pjazJhOtquoRym5wxwGsYSW53pAzJ47Juz4mcgtmecpLFawmm-zQhzq-oVCSUDxEsT5AVQyspdXZ037AHSToy0ry5KTdt8k1xNMjOu8QURDPtXEOUJ7pM1_RW_Oe3tECVhvR9yOQvnF2xuiDYpgNAdQY0SMG53Dd9pQwI806n7N14eU5uBg6hX1Up48FrvA4UwjjvBBkob3e3FiaLPgM1c_OXOynWI7YpeuH7TSTQWJgPpPFJBhVM4bAy4Em7u-KrIW6PLZatGJwX-JE1Cfq5DMt4v7OoF-ipP2B5u3_qsCf.YCwDoNtW9hpVmma2qsNuQ-KsASJ6b93zRxl6tggoxIA&dib_tag=se&keywords=miuzei+25kg+servo&qid=1736648634&sprefix=miuzei+25%2Caps%2C233&sr=8-5) (or MG996R or similar) + supplied screws + round servo horn
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
| <img width="100" alt="Servo_Frame_Mount_Clamp_Insert" src="https://github.com/user-attachments/assets/c4f4a299-49c2-4280-9b61-5a2158216f7c" /> | Press fit extrusion slot clamp inserts for the actuator servo mount | [stl](https://github.com/weuzor/bowden_cutter/blob/main/STL/Actuator%20Parts/Servo_Frame_Mount_Clamp_Insert_x2.stl) | [step](https://github.com/weuzor/bowden_cutter/blob/main/CAD/Actuator%20Parts/Servo_Frame_Mount_Clamp_Insert_x2.step) |
| <img width="100" alt="Wire_Puller" src="https://github.com/user-attachments/assets/b636efdd-fa4a-4a45-bc94-c9c16d2ef66e" /> | wire pulling servo attachment| [stl](https://github.com/weuzor/bowden_cutter/blob/main/STL/Actuator%20Parts/Wire_Puller.stl) | [step](https://github.com/weuzor/bowden_cutter/blob/main/CAD/Actuator%20Parts/Wire_Puller.step) |
### Assembly
<img width="200" alt="actuator_body" src="https://github.com/user-attachments/assets/d5922760-ac2b-4eee-b079-ff1ca9ba5038" />
<img width="200" alt="actuator_puller" src="https://github.com/user-attachments/assets/54071c3e-76d2-4f79-a27c-11835c298704" />
<img width="200" alt="actuator_servoy" src="https://github.com/user-attachments/assets/6603d521-6a93-4eaa-b773-dcf1c5fdcd0b" />
<img width="200" alt="actuator_wire" src="https://github.com/user-attachments/assets/285d378b-fa9a-4ebf-b4ba-dc3898706fe0" />



