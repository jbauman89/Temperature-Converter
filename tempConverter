import Foundation
enum TempConverter
{
    case Fahrenheit
    case Celsius
    

        init(in scale: String)
        {
            self = .Fahrenheit
            if scale.contains("f"){
                self = .Celsius
                }
            
            else if scale.contains("c"){
                self = .Celsius
                }
        }
    
    func convert(for temp: Double)
    {
        switch(self)
        {
        case .Fahrenheit: print("\(temp)° in Fahrenheit is \((temp - 32) * 5 / 9)° in Celsius")
            break
        case .Celsius: print("\(temp)° in Celsius is \((temp * 9) / 5 + 32)° in Fahrenheit")
            break
        }
    }
    
    mutating func switchScale()
    {
        switch(self)
        {
        case .Fahrenheit:
            self = .Celsius
            convert(for: temp)
            break
            
        case .Celsius:
            self = .Fahrenheit
            convert(for: temp)
            break
        }
    }
}

// intentional typo of 'celsius'
var tempDemo = TempConverter(in: "celcius")


var temp = 100.0

tempDemo.convert(for: temp)

tempDemo.switchScale()



temp = 212.0

tempDemo.convert(for: temp)

tempDemo.switchScale()
