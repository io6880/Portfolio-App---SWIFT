# Portfolio-App---SWIFT

I have attahced the project into this repository. I am also copy pasting my code into this readme fole for your kind perusal.

import SwiftUI

struct ContentView: View {
    var body: some View {
        VStack (spacing:20){
            HStack{
                Text("Irfan Mohammed O.K").font(.largeTitle).bold().foregroundColor(Color(UIColor.systemIndigo))
                Spacer()
                Text("...").foregroundColor(Color(UIColor.systemIndigo))
            }
            
            HStack{
                Image("Subject").resizable().aspectRatio(contentMode: .fill).frame(width: 80,height: 80).clipShape(Circle())
                Spacer()
                VStack(alignment: .leading){
                    Text("IOS APP Developer").foregroundColor(Color(UIColor.systemIndigo)).font(.headline).fontWeight(.heavy)
                    ZStack (alignment: .leading){
                        Rectangle().frame(width:110,height: 10).opacity(0.3).foregroundColor(Color(UIColor.systemIndigo))
                        
                        Rectangle().frame(width: 110,height: 10).foregroundColor(Color(UIColor.systemIndigo))
                        
                    }.cornerRadius(45).foregroundColor(Color(UIColor.systemIndigo))
                    
                    HStack{
                        Text("10").foregroundColor(Color(UIColor.systemIndigo)).font(.headline).fontWeight(.heavy)
                        Text("Just started the journey").foregroundColor(.secondary)
                    }
                }
                
                Spacer()
                Image(systemName: "square.and.arrow.up").foregroundColor(.red).padding().background(Color.red.opacity(0.1)).cornerRadius(12)
                
            }.padding(.vertical, 8)
            
            
            HStack{
                Button(action:{}){
                    Text("Achievements").foregroundColor(.white).bold().padding(.vertical,10).frame(width:130).padding(.all,8)
                }.background(Color(UIColor.systemIndigo)).clipShape(Capsule())
                
                
                Button(action:{}){
                    Text("Coding").foregroundColor(Color(UIColor.systemIndigo)).bold().padding(.vertical,10).frame(width:90).padding(.all,8)
                }.background(Color.clear).clipShape(Capsule())
                
                Button(action:{}){
                    Text("Projects").foregroundColor(Color(UIColor.systemIndigo)).bold().padding(.vertical,10).frame(width:90).padding(.all,8)
                }.background(Color(UIColor.clear)).clipShape(Capsule())
                
            }.clipShape(Capsule()).overlay(RoundedRectangle(cornerRadius: 40).stroke(Color.gray.opacity(0.5), lineWidth:0.5 )).padding(.top,10)
            
            
            HStack(spacing: 15){
                Image(systemName: "hexagon").resizable().frame(width:20, height: 20).padding().background(Color.white).cornerRadius(100).foregroundColor(Color(UIColor.systemIndigo))
                
                VStack(alignment: .leading, spacing:12){
                    Text("Princess Diana Award").foregroundColor(Color(UIColor.systemIndigo)).font(.headline)
                    Text("From the British Royal Family").foregroundColor(.secondary).lineLimit(1).font(.subheadline)
                }
                Spacer()
                
                Text("").foregroundColor(Color.secondary).opacity(0.5)
            }.padding().background(Color.gray.opacity(0.1)).cornerRadius(20)
            
            HStack(spacing: 15){
                Image(systemName: "triangle").resizable().frame(width:20, height: 20).padding().background(Color.white).cornerRadius(100).foregroundColor(Color(UIColor.systemIndigo))
                
                VStack(alignment: .leading, spacing:12){
                    Text("TEDx Speaker").foregroundColor(Color(UIColor.systemIndigo)).font(.headline)
                    Text("I gave a TED talk at TEDxOOBSCHOOL").foregroundColor(.secondary).lineLimit(1).font(.subheadline)
                }
                Spacer()
                
                Text("").foregroundColor(Color.secondary).opacity(0.5)
            }.padding().background(Color.green.opacity(0.1)).cornerRadius(20)
            
            HStack(spacing: 15){
                Image(systemName: "circle").resizable().frame(width:20, height: 20).padding().background(Color.white).cornerRadius(100).foregroundColor(Color(UIColor.systemIndigo))
                
                VStack(alignment: .leading, spacing:12){
                    Text("Professional Cyclist").foregroundColor(Color(UIColor.systemIndigo)).font(.headline)
                    Text("I cycled across an entire country").foregroundColor(.secondary).lineLimit(1).font(.subheadline)
                }
                Spacer()
                
                Text("").foregroundColor(Color.secondary).opacity(0.5)
            }.padding().background(Color.red.opacity(0.1)).cornerRadius(20)
            
            HStack(spacing: 15){
                Image(systemName: "square").resizable().frame(width:20, height: 20).padding().background(Color.white).cornerRadius(100).foregroundColor(Color(UIColor.systemIndigo))
                
                VStack(alignment: .leading, spacing:12){
                    Text("Half Marathon").foregroundColor(Color(UIColor.systemIndigo)).font(.headline)
                    Text("Completed a half marathon at 16").foregroundColor(.secondary).lineLimit(1).font(.subheadline)
                }
                Spacer()
                
                Text("").foregroundColor(Color.secondary).opacity(0.5)
            }.padding().background(Color.blue.opacity(0.1)).cornerRadius(20)
        }
    }
}

struct ContentView_Previews: PreviewProvider {
    static var previews: some View {
        ContentView()
    }
}
