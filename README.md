# MelodyLab v5.116 Speed of Sound Extra Slow Motion

ปรับหน้า Displacement and Pressure ให้กราฟกินพื้นที่แนวตั้งเต็มขึ้นบนจอมือถือ
- เพิ่มความสูง canvas สำหรับหน้า Displacement and Pressure / Longitudinal
- ขยายความสูงของกราฟบน-ล่างให้ใช้พื้นที่เกือบเต็ม slot
- ลดช่องว่างใต้กราฟล่าง
- คงพฤติกรรมความถี่, แอมพลิจูด, อัตราเร็วคลื่น, เฟส และความต่างเฟส

## v5.116 Speed of Sound Extra Slow Motion
- เลื่อน badge “Phase Difference: Δφ = ...°” ลงมาอยู่ในกรอบกราฟการกระจัด
- แก้ไม่ให้ข้อความ Phase Difference ซ้อนทับกับลูกศรทิศทางการเคลื่อนที่ของคลื่น
- คงการขยายกราฟแนวตั้งและการปรับความถี่ f จาก v5.116

## v5.116 Speed of Sound Extra Slow Motion
- ปรับกราฟ Longitudinal Wave ให้อนุภาคสั่นซ้าย–ขวารอบตำแหน่งสมดุล
- เพิ่มจุดสมดุลสีจางและจุดจริงของอนุภาค เพื่อให้เห็นว่าอนุภาคไม่ได้ไหลไปกับคลื่น
- แสดงส่วนอัด–ส่วนขยายจากความหนาแน่นของอนุภาค
- เพิ่มลูกศร “การสั่นของอนุภาค” ที่จุดสังเกต
- แก้ให้ f และ v ส่งผลต่อความยาวคลื่นของหน้า Longitudinal Wave ผ่าน λ = v/f
- คงหน้า Displacement and Pressure จาก v5.116


## v5.116 Speed of Sound Extra Slow Motion
- ลบหัวข้อ Longitudinal / Transverse ออกจากเมนู Wave Visualizer
- เพิ่มหัวข้อใหม่ Speed of Sound (อัตราเร็วเสียง)
- ภาพจำลองใหม่แสดงแหล่งกำเนิดเสียง ไมโครโฟน ระยะทาง d เวลาที่เสียงเดินทาง Δt และอัตราเร็วเสียง v
- ใช้ความสัมพันธ์ v = d / Δt และ v ≈ 331 + 0.6T
- เพิ่มการส่งออกข้อมูลของหัวข้อ Speed of Sound Extra Slow Motion ตามชื่อหัวข้อ

## v5.116 Speed of Sound Extra Slow Motion
- ปรับหน้า Speed of Sound เป็นสื่อการสอนฟิสิกส์ชัดเจน
- แสดงแหล่งกำเนิดเสียง ไมโครโฟน พัลส์เสียง เส้นระยะทาง d ค่า Δt และสูตร v = d/Δt
- เพิ่มตัวควบคุม Distance d, Temperature T, Time Speed และแสดงค่า v, Δt อัตโนมัติ
- คงการลบหัวข้อ Longitudinal / Transverse ออกจากเมนู Wave Visualizer

## v5.116 Speed of Sound Extra Slow Motion
- ปรับหน้า Speed of Sound ให้ใช้รูปแบบเดียวกับ Longitudinal, Pressure, Displacement and Pressure
- ใช้ class ชุด visualizerTemplatePage / longitudinalFocusPage / longitudinalFocusGrid / longitudinalMainViz / neonControlViz
- ใช้ปุ่มเล่น หยุด รีเซ็ต และปุ่มส่งออกแบบเดียวกับสามหน้าหลัก
- ใช้รูปแบบพารามิเตอร์แบบ neonParamRow เดียวกัน
- คงภาพจำลองอัตราเร็วเสียงและสมการ v = d/Δt, v = 331 + 0.6T

## v5.116 Speed of Sound Extra Slow Motion
- เปลี่ยนสัญลักษณ์ระยะทางจาก d เป็น s ในหน้า Speed of Sound
- ปรับสูตรเป็น v = s / Δt
- ปรับ Time Speed ให้ช้าลง ค่าเริ่มต้น 0.10× ช่วง 0.03×–1.00×
- เพิ่ม slow-motion display factor เพื่อให้เห็นการเดินทางของพัลส์เสียงชัดขึ้น โดยค่าฟิสิกส์ v และ Δt ยังคำนวณจริง
- เพิ่ม export alias parameter_path_length_s_m

## v5.116 Speed of Sound Extra Slow Motion
- ปรับพัลส์เสียงให้ช้าลงกว่ารอบ v5.116
- Time Speed ค่าเริ่มต้น 0.05× ช่วง 0.01×–0.50×
- เพิ่ม slow-motion display factor จาก 10 เป็น 40 เพื่อให้เห็นการเดินทางของพัลส์เสียงชัดขึ้นมาก
- ค่าฟิสิกส์ v และ Δt ยังเป็นค่าจริง ไม่ได้ถูกทำให้ช้าตามภาพ

## v5.116 Add Sound Topics
- เพิ่ม 7 หัวข้อเสียงใน Wave Visualizer ต่อจาก Speed of Sound พร้อมหน้าเบื้องต้นและภาพจำลอง canvas

## v5.116 Physics Checked Sound Topics
- จัดเมนู Wave Visualizer ตามแผนที่ 1–13 รวม 21 หัวข้อ และปรับหัวข้อ 5–21 ตามหลักฟิสิกส์ก่อนลงโค้ด

## v5.116 Reflection Echo Audio
- แก้ init() ไม่ให้หน้า Visualizer ย่อย crash จากปุ่ม/element ของหน้าวัดเสียงที่ไม่มีในหน้านั้น
- ทำปุ่มเล่น/หยุด/รีเซ็ต/บันทึก PNG ให้ null-safe
- เพิ่ม listener ให้ slider หัวข้อใหม่ครบ เช่น mode, length, source level, protection
- คงเมนู Wave Visualizer 21 หัวข้อจาก v5.116

## v5.116 Reflection Echo Audio
- แก้หัวข้อใหม่ให้มี animation จริงเมื่อกด Play
- ปรับ slider ให้มีผลต่อภาพจำลอง เช่น มุมสะท้อน ช่องเปิด ระยะห่างแหล่งกำเนิด โหมดท่อ เลขมัค ระดับเสียง
- กด Play/Pause/Reset แล้ว redraw ทันที
- คงเมนู 21 หัวข้อและ runtime fix จาก v5.116

## v5.116 Reflection Echo Audio
- ตรวจครบ 21 หัวข้อใน Wave Visualizer
- เพิ่ม/ซ่อมพารามิเตอร์ให้หัวข้อ 5–21 ปรับได้จริงตามภาพจำลอง
- เพิ่ม input/change listener ให้ range และ select ทุกหัวข้อ
- เพิ่ม session.html redirect ป้องกันลิงก์บันทึกผลเดิมเป็น 404

## v5.116 Reflection Echo Audio
- คง 4 หน้าแรกไว้เป็นแม่แบบ ไม่แก้โครงหลัก
- Rebuild หัวข้อ 5–21 ใหม่ให้ใช้ layout/control/export แบบเดียวกับ 4 หน้าแรก
- เพิ่มรายละเอียดฟิสิกส์และกราฟ/แถบค่าใน canvas ให้สื่อความหมายมากขึ้น
- ทุกหัวข้อมี Play/Pause/Reset, parameter control, canvas animation และ export

## v5.116 Reflection Echo Audio
- แก้การสั่นพ้องของอากาศในท่อให้คำนวณ fₙ ตามหลักฟิสิกส์:
  - ท่อเปิดสองด้าน: fₙ = nv/(2L)
  - ท่อปิดหนึ่งด้าน: fₙ = (2n−1)v/(4L)
- เพิ่มสูตร Doppler สำหรับผู้สังเกตนิ่ง:
  - ด้านหน้า: f′ = f v/(v−vₛ)
  - ด้านหลัง: f′ = f v/(v+vₛ)
- คง 4 หน้าแรกและ template ของ v5.116

## v5.116 Reflection Echo Audio
- เพิ่ม listener ที่ตกหล่นสำหรับ Beats และ Harmonics/Timbre: vizFreq2, vizHarmonicMix, vizInstrument
- ตรวจซ้ำครบ 21 หัวข้อ ทั้ง runtime, parameter listener, internal links และสูตรฟิสิกส์หลัก

## v5.116 Reflection Echo Audio
- แก้บั๊กสำคัญ: drawVisualizer วิ่งเข้า renderer เก่า (drawSoundTopicPlaceholder) ก่อน renderer ใหม่
- ให้หัวข้อ 5–21 ใช้ drawRebuiltTopic โดยตรง
- กด Play/Reset จะ cancel animation frame เดิมก่อนเริ่มใหม่ ลดปัญหาลูปซ้อน

## v5.116 Reflection Echo Audio
- กู้ app.js กลับจากฐานเต็มที่มีตัวแปรและฟังก์ชันหลักครบ เช่น $, vizState, getVizParams, drawSpeaker, roundRect
- คงหน้า HTML/เมนู/หัวข้อ 5–21 จาก v5.116
- ให้หัวข้อ 5–21 เข้า drawRebuiltTopic โดยตรง ไม่ผ่าน placeholder เก่า
- แก้ปุ่ม Play/Reset ให้เริ่ม animation loop ใหม่ได้

## v5.116 Reflection Echo Audio
- เริ่ม rebuild แบบทีละหน้า โดยหน้า 5 Sound Reflection ยึด mockup เป็นหลัก
- เพิ่ม ray labels, normal line, angle arcs, formula badge, wall texture, reflection strength และ wavefronts
- เพิ่ม Wall Type และ Amplitude control เพื่อให้ตรงกับ reference มากขึ้น
- คง runtime เต็มจาก v5.116

## v5.116 Reflection Echo Audio
- เปลี่ยนคำว่า เส้นตั้งฉาก -> เส้นแนวฉาก
- ปรับตำแหน่งเส้นแนวฉากให้ผ่านจุดตกกระทบอย่างชัดเจน
- ปรับเรขาคณิตรังสีให้สัมพันธ์กับลำโพงมากขึ้น
- แสดงค่ามุมตกกระทบและมุมสะท้อนเป็นตัวเลขบนสื่อ
- เมื่อเลือกผนังแบบดูดซับ จะลดความเข้มและขนาดของรังสีสะท้อนเพื่อสื่อการสูญเสียพลังงาน

## v5.116 Reflection Echo Audio
- เพิ่มคลื่นสะท้อนสีเขียวที่เริ่มจากจุดตกกระทบบนผนัง แล้วแผ่ออกจากผนังกลับเข้าสู่อากาศ
- ปรับคำอธิบาย Echo path ให้สื่อว่าเป็นคลื่นสะท้อนออกจากผนัง ไม่ใช่คลื่นที่ยังวิ่งเข้าหาผนัง
- ผนังดูดซับยังลดความเข้ม/ความหนาของคลื่นสะท้อนและรังสีสะท้อน

## v5.116 Reflection Echo Audio
- หน้า Sound Reflection เอา slider ความถี่ออก เพราะการสะท้อนของเสียงไม่ทำให้ความถี่เปลี่ยน
- แสดง Frequency f เป็นค่า/ข้อความคงที่แทน: f คงที่
- ปรับ Amplitude A ให้เห็นผลชัดขึ้นกับความหนา ความสว่าง ขนาดจุดพลังงาน และ wavefront
- พลังงานสะท้อนกลับแสดงโดยประมาณตาม A² และชนิดผนัง

## v5.116 Reflection Echo Audio
- เพิ่ม Distance to Wall d
- คำนวณ t_echo = 2d/343
- แสดงสถานะ ✅ เกิด Echo / ⚠️ ไม่เกิด Echo โดยใช้เกณฑ์ 0.10 s
- เพิ่มปุ่ม Play Echo Demo เพื่อฟังเสียงจริงตามค่า d, A และชนิดผนัง
- ใช้คำว่า “ไม่เกิด Echo” ในเชิงการได้ยิน: เสียงสะท้อนยังมีอยู่ แต่หูยังแยกไม่ออกเป็น Echo ชัดเจน

## v5.116 Echo Threshold Complete
- ปรับสัญลักษณ์ระยะทางในหน้า Sound Reflection จาก d เป็น s ให้ตรงกับที่ใช้ในบทเรียนก่อนหน้า
- แสดง Distance to Wall s
- แสดงสูตร t_echo = 2s/v หรือ 2s/343
- คง id ภายในเป็น vizDistance เพื่อไม่กระทบระบบเดิม

## v5.116 Echo Threshold Complete
- เพิ่มข้อความหมายเหตุว่าเสียงสะท้อนยังมีอยู่ แต่ถ้า t_echo < 0.10 s หูรับรวมกับเสียงเดิม จึงไม่เกิด Echo ในเชิงการได้ยิน
- เพิ่มเกณฑ์ Echo ≈ 0.10 s ในกล่องสถานะ
- เพิ่มระยะเริ่มเกิด Echo s ≈ 17.2 m จาก s = vt/2
- คงปุ่ม Play Echo Demo และใช้สูตร t_echo = 2s/v


## v5.116 Reflection Layout Echo Fix
- จัดองค์ประกอบหน้า Sound Reflection ใหม่ให้ไม่รกบนจอมือถือ
- ย้ายชนิดผนังไปไว้ด้านบนของผนัง
- ทำเส้น Normal line ให้เด่นและใช้เป็นเส้นอ้างอิงหลัก
- ขยายมุมการแสดงคลื่นสะท้อนให้เกินแนวรังสีตกกระทบ
- ปรับเสียง Echo Demo เป็นเสียงคล้ายการตบมือเพื่อฟังเสียงก้องชัดขึ้น
- เปลี่ยนสัญลักษณ์ระยะจาก d เป็น s ในหน้า Reflection

## v5.116 Clean Release
- ทำไฟล์ปล่อยจริงแบบสะอาด
- ลบไฟล์รายงานตรวจรุ่นเก่าออกจาก zip
- ปรับ meta build version ทุกหน้าให้ตรงกันเป็น v5.116-clean-release
- คงการแก้หน้า Sound Reflection รอบก่อนหน้าไว้ครบถ้วน
- เพิ่มคำแนะนำใกล้ปุ่มเสียง: ตั้ง s > 20 m เพื่อฟัง Echo ชัด
- cache: melodylab-v5-116-clean-release
