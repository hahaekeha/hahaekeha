import speech_recognition as sr
import pyttsx3
import datetime
import wikipedia
import webbrowser
import os
import time
import subprocess
from ecapture import ecapture as ec
import wolframalpha
import json
import requestsengine=pyttsx3.init('sapi5')
voices=engine.getProperty('voices')
engine.setProperty('voice','voices[0].id')
def speak(text):
    engine.say(text)
    engine.runAndWait()
	
def wishMe():
    hour=datetime.datetime.now().hour
    if hour>=0 and hour<12:
        speak("Hello,Good Morning")
        print("Hello,Good Morning")
    elif hour>=12 and hour<18:
        speak("Hello,Good Afternoon")
        print("Hello,Good Afternoon")
    else:
        speak("Hello,Good Evening")
        print("Hello,Good Evening")
			
def wishMe():
    hour=datetime.datetime.now().hour
    if hour>=8:30 and hour<16:20:
        speak("How is school going")
        print("How is school going")
    elif hour>=12 and hour<18:
        speak("Are you finisched with school yet?")
        print("Are you finisched with school yet?")
    else:
        speak("Hello,Good Evening")
        print("Hello,Good Evening")
		def takeCommand():
    r=sr.Recognizer()
    with sr.Microphone() as source:
        print("Listening...")
        audio=r.listen(source)
  elif "weather" in statement:
            api_key="Apply your unique ID"
            base_url="https://api.openweathermap.org/data/2.5/weather?"
            speak("what is the city name")
            city_name=takeCommand()
            complete_url=base_url+"appid="+api_key+"&q="+city_name
            response = requests.get(complete_url)
            x=response.json()
            if x["cod"]!="404":
                y=x["main"]
                current_temperature = y["temp"]
                current_humidiy = y["humidity"]
                z = x["weather"]
                weather_description = z[0]["description"]
                speak(" Temperature in kelvin unit is " +
                      str(current_temperature) +
                      "\n humidity in percentage is " +
                      str(current_humidiy) +
                      "\n description  " +
                      str(weather_description))
                print(" Temperature in kelvin unit = " +
                      str(current_temperature) +
                      "\n humidity (in percentage) = " +
                      str(current_humidiy) +
                      "\n description = " +
                      str(weather_description))
  elif "log off" in statement or "sign out" in statement:
            speak("Ok , your pc will log off in 10 sec make sure you exit from all applications")
            subprocess.call(["shutdown", "/l"])
			
time.sleep(3)

        try:
            statement=r.recognize_google(audio,language='en-in')
            print(f"user said:{statement}\n")

        except Exception as e:
            speak("Pardon me, please say that again")
            return "None"
        return statement

print("Loading your AI personal assistant Jan-pieter")
speak("Loading your AI personal assistant Jan-pieter")
wishMe()
if __name__=='__main__':


    while True:
        speak("Tell me how can I help you now?")
        statement = takeCommand().lower()
        if statement==0:
		if "good bye" in statement or "ok bye" in statement or "stop" in statement:
            speak('your personal assistant Jan-pieter is shutting down,Good bye')
            print('your personal assistant Jan-pieter is shutting down,Good bye')
            break
			def wishMe():
    question=question.question.now().assistant
    if question is ''microphone on'':
        ''microphone on'' switch sr.Microphone on.takeCommand
    elif hour>=12 and hour<18:
        speak("Hello,Good Afternoon")
        print("Hello,Good Afternoon")
    else:
        speak("sorry, i didn't understand that")
        print("sorry, i didn't understand that")
		uestion=question.question.now().assistant
    
    else:
        speak("sorry, i didn't understand that")
        print("sorry, i didn't understand that")
		
		elif 'open youtube' in statement:
            webbrowser.open_new_tab("https://www.youtube.com")
            speak("youtube is open now")
            time.sleep(5)

        elif 'open google' in statement:
            webbrowser.open_new_tab("https://www.google.com")
            speak("Google chrome is open now")
            time.sleep(5)

        elif 'open gmail' in statement:
            webbrowser.open_new_tab("gmail.com")
            speak("Google Mail open now")
            time.sleep(5)
			elif 'open magister' in statement:
            webbrowser.open_new_tab("https://trevianum.magister.net/magister")
            speak("magister is open now")
            time.sleep(5)
            elif 'rollercoaster time' in statement:
                 webbrowser.open_new_tab("https://www.youtube.com/user/ThemeParkWorldwide")
                   speak("themepark worldwide is now open ")
                    time.sleep(5
  elif 'Jan-pieter' in statement:
            webbrowser.open_new_tab("https://www.youtube.com/watch?v=awXuLgKbEbM")
            speak("Yes sir")
            time.sleep(5)
