# Assigment-2
func rightTriangle(num:Int){
  for i in 1...num{
    for j in 1...i{
      print(" *",terminator:"")
    }
    print()
  }
}
print("Enter number for pattern")
var no=Int(readLine() ?? "0") ?? 0
print("Right Triangle")
rightTriangle(num:no)

func pyramid(num:Int){
  for i in 0...num{
    for k in stride(from:0 ,to:num-i ,by:1){
       print(" ",terminator:"")
     }
    for k in 0...i{
      print(" *",terminator:"")
    }
    print()
  }
}
print("Pyramid")
pyramid(num:no)
func MirroredRightTriangle(num:Int){
  
  for i in 1...num{
    for k in 0...num-i{
      print("  ",terminator:"")
    }
    for j in 1...i{
      print(" *",terminator:"")
    }
    print()
  }
}
print("Mirrored Right Triangle")
MirroredRightTriangle(num:no)

func Diamond(num:Int){
  var n=0
  for i in 0...num-1{
    for j in 0...num-i{
      print(" ",terminator:"")
    }
    for k in 0...i{
      print(" *",terminator:"")
    }
    print()
  }
  for i in stride(from: num-1, to: 0, by: -1){
    for j in 0...num-i+1{
      print(" ",terminator:"")
    }
    for k in stride(from: i,to:0,by: -1){
      print(" *",terminator:"")
    }
    print()
  }
}
print("4) Diamond")
Diamond(num:no)


 func DownwardTriangle(num:Int){
  for i in stride(from:num, to:0,by:-1){
    for j in stride(from: i,to:0,by:-1){
      print(" *",terminator:"")
    }
    print()
 }
 }

print("5) Downward Triangle")
DownwardTriangle(num:no)

func RightPascalTriangle(num:Int){
  for i in 1...num{
    for j in 1...i{
      print(" *",terminator:"")
    }
    print()
  }
  for i in stride(from:num-1, to:0,by:-1){
    for j in stride(from: i,to:0,by:-1){
      print(" *",terminator:"")
    }
    print()
 }
}
print("6) Right Pascal’s Triangle")
RightPascalTriangle(num:no)

func SandglassPattern(num:Int){
  
  for i in stride(from:num, to:0,by:-1){
    for k in stride(from:0 ,to:num-i ,by:1){
      print(" ",terminator:"")
    }

    for j in stride(from: i,to:0,by:-1){
      print(" *",terminator:"")
    }
    print()
 }
  for i in 1...num-1{ 
    for k in stride(from:num-i-1 ,to:0 ,by:-1){
      print(" ",terminator:"")
    }
    for j in 0...i{
      print(" *",terminator:"")
    }
    print()
  }
}

print("7) Sandglass Pattern")
SandglassPattern(num:no)
