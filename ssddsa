from kivy-app import App from kivy-vix.screenmanager import ScheenManagen. Screen from kivy.uix.boxlayout import BoxLayout from kivy uix. label import Label from kivy.vix.button import Button from kivy-vix. textinput import TextInput from kivy.core.window import Window from kivy.vix.scrollview import Scrolliew
from instructions import txt_instruction, txt_test1, txt_test2, txt_test3, txt_sits from ruffier import test
age = 7
name = "™
p1, р2, р3 = 0, 0, 0
class InstrScr(Screen): 1 usage def __init__(self, **kwargs):
super ().__init__ (**kwargs)
instr = Label(text=txt_instruction)
Lb11 = Label(text='Введите имя:". halign='night)
self. in_name = TextInput(multiline=False)
Lb12 = Label(text='Введите возраст:", halign= night')
self.in_age = TextInput(text='7', multiline=False)
self.btn = Button(text='Начать, size_hint=(0.3. 0.2), pos_hint=(*center_x': 0.57)
self.btn.on_press = self.next
Line1 = BoxLayout(size_hint=(0.8, None), height=' 30sp')
Line2 = BoxLayout(size_hint=(0.8, None), height='30sp' )
Line1. add _widget (Lbl1)
Linel. add _widget (self.in_name)|
class InstrScr(Screen): 1 usage def -_init__ (self, **kwargs):
linel. add_widget (Lbl1)
Linel. add_widget (self.in_name)
line2.add_widget (lbl2)
Line2. add_widget(self.in_age)
outer = BoxLayout(orientation='vertical', padding=8, spacing=8)
outer.add _widget(instr)
outer .add_widget(line1)
outer.add_widget (line2)
outer. add_widget(self.btn)
self.add _widget(outer)
def next(self): 4 usages (3 dynamic)
global name
name = self.in_name.text
self.manager.current = 'pulsel'
class PulseScr(Screen): 1 usage def __init__ (self, **kwargs) :
super ().__init__(**kwargs)
instr = Label(text=txt_test1)
Line = BoxLayout(size_hint=(0.8, None), height= 30sp' )
lbl_result = Label(text='Введите результат:", halign=right')
self.in_result = TextInput(text='0', multiline=False)
line. add_widget(lbl_result)
line. add_widget(self.in_result)
self.btn = Button(text="Продолжить", size_hint=(0.3, 0.2), pos_hint=('center_x': 0.5})
self.btn.on_press = self.next
outer = BoxLayout(orientation='vertical'. padding=8, spacing=8)
outer.add
widget (instr)
outer .add_widget(line)
outer.add_widget(self.btn)
self.add_widget (outer)
def next(self): 4 usages (3 dynamic)
global pl
p1 = int(self.in_result.text)
self.manager.current = 'sits'
class CheckSits (Screen): 1 usage def __init__(self, **kwargs) :
super).-_init__ (**kwargs)
instr = Label(text=txt_sits)
self.btn = Button(text='Продолжить'. size_hint=(0.3, 0.2), pos_hint={'center_x': 0.5})
self.btn.on_press = self.next
outer = BoxLayout (orientation='vertical'. padding=8, spacing=8)
outer .add_widget(instr)
outer .add_widget(self.btn)
self.add_widget (outer)
def next(self): 4 usages (3 dynamic)
self.manager.current = 'pulse2'
class PulseScr2(Screen): 1 usage def__init__(self, **kwargs) :
super).__init_(**kwargs)
instr = Label(text=txt_test3)
Linel = BoxLayout(size_hint=(0.8, None). height=' 30sp')
lbl_resultl = Label(text= 'Результат:'. halign='right')
self.in_resultl = TextInput(text='0'
. multiline=False)
linel.add_widget (Lbl_result1)
Linel.add_widget(self.in_result1)
Line2 = BoxLayout(size_hint=(0.8, None), height=^30sp')
lbl_result2 = Label (text='Результат после отдыха:', halign='right')
self.in_result2 = TextInput(text='0*. multiline=False)
Line2.add_widget (Ibl_nesult2)
line2.add_widget(self.in_result2)
self.btn = Button(text='Завершить". size_hint=(0.3, 0.2), pos_hint=('center_x': 0.5})
self.btn.on_press = self.next
outer = BoxLayout(orientation='vertical'. padding=8, spacing=8)
outer .add_widget(instr)
outer.add_ widget (line1) outer .add_widget(line2)
outer .add_widget(self.btn)
self.add_widget (outer)
def next(self): 4 usages (3 dynamic)
global p2, ps
p2 = int(self.in_result1.text)
p3 = int(self.in_result2.text)
self .manager.current = result'
class Result(Screen): 16 usages (15 dynamic)
def __init__(self. **kwargs):
super (.__init_ (**kwargs)
self.outer = BoxLayout(orientation='vertical', padding=8, spacing=8)
self.instr = Label (text = '')
self.outer add_widget(self.instr)
self.add_widget(self.outer)
self.on_enter = self. before
def before(self): 19 usages (18 dynamic)
global name
self.instr.text = name + '\n' + test(pl. p2, p3, age)
class HeartCheck(App) : 1 usage
def build (self): 6 usages (6 dynamic)
sm = ScreenManager ()
sm. add_widget (InstrScr(name='instr'))
sm. add_widget (PulseScr (name= 'pulsel'))
sm.add_widget (CheckSits (name='sits'))
sm. add_widget(PulseScr2(name='pulse2'))
sm.add_widget (Result (name='result'))
return sm
app = HeartCheck(
app. run ()
