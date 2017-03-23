unit Unit1;

{$mode objfpc}{$H+}

interface

uses
  Classes, SysUtils, FileUtil, Forms, Controls, Graphics, Dialogs, StdCtrls;

type

  { TForm1 }

  TForm1 = class(TForm)
    Button1: TButton;
    Button2: TButton;
    Button3: TButton;
    CheckBox1: TCheckBox;
    CheckBox2: TCheckBox;
    Edit1: TEdit;
    Edit2: TEdit;
    Edit3: TEdit;
    Edit4: TEdit;
    Label1: TLabel;
    Label2: TLabel;
    Label3: TLabel;
    Label4: TLabel;
    Label5: TLabel;
    Label6: TLabel;
    Label7: TLabel;
    Label8: TLabel;
    RadioButton1: TRadioButton;
    RadioButton2: TRadioButton;
    procedure Button1Click(Sender: TObject);
    procedure Button2Click(Sender: TObject);
    procedure Button3Click(Sender: TObject);
    procedure Label2Click(Sender: TObject);
  private
    { private declarations }
  public
    { public declarations }
  end;

var
  Form1: TForm1;
   a1, a2, b1, b2, s1, s2 : real;
implementation

{$R *.lfm}

{ TForm1 }

procedure TForm1.Button1Click(Sender: TObject);
begin
  a1 := StrToFloat (Edit1.Text);
  b1 := StrToFloat (Edit2.Text);
  a2 := StrToFloat (Edit3.Text);
  b2 := StrToFloat (Edit4.Text);
  s1 := a1*b1;
  s2 := a2*b2;
 if a1>a2 then Label5.Caption :='Перший прямокутник площею' +FloatToStr (s1) + #13 + ' більший за другий рямокутник площею ' + FloatToStr (s2)
 else
   if s1=s2 then Label5.Caption :='Прямокутники рівні, їх площа =' + FloatToStr(s1)
   else Label5.Caption :='Другий прямокутник площею' +FloatToStr (s2) + #13 + ' більший за перший рямокутник площею ' + FloatToStr (s1);
end;

procedure TForm1.Button2Click(Sender: TObject);
begin
  a1 := StrToFloat (Edit1.Text);
  b1 := StrToFloat (Edit2.Text);
  a2 := StrToFloat (Edit3.Text);
  b2 := StrToFloat (Edit4.Text);
  If (CheckBox1.Checked=True) and (a1=b1)
  then Label7.Caption := 'Квадрат'
  else
  if CheckBox1.Checked =False
  then Label7.Caption :='     '
    else Label7.Caption :='Прямокутник';
  If (CheckBox2.Checked=True) and (a2=b2) then Label8.Caption := 'Квадрат'
  else
    if CheckBox2.Checked = False then Label8.Caption :='     '
    else Label8.Caption :='Прямокутник';

end;

procedure TForm1.Button3Click(Sender: TObject);
begin
  a1 := StrToFloat (Edit1.Text);
  b1 := StrToFloat (Edit2.Text);
  a2 := StrToFloat (Edit3.Text);
  b2 := StrToFloat (Edit4.Text);
  if RadioButton1.Checked = True then
  if ((a1<=a2) and (b1<=b2)) or ((a1<=b2) and (b1<=a2)) then
  Label5.Caption := 'Перший прямокутник розміститься' +#13+ 'у середині другого'
  else Label5.Caption :='Перший прямокутник не розміститься' +#13+ 'у середині другого';
  if RadioButton2.Checked = True then
  if ((a1<=a2) and (b1<=b2)) or ((a1<=b2) and (b1<=a1)) then
  Label5.Caption := 'Другий прямокутник розміститься' +#13+ 'у середині прешого'
  else Label5.Caption :='Другий прямокутник не розміститься' +#13+ 'у середині першого';
end;

procedure TForm1.Label2Click(Sender: TObject);
begin

end;

end.

