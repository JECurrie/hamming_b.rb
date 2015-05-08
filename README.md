# hamming_b.rb
class Hamming
	def self.compute(x, y)

    xx = Array.new
    yy = Array.new

    xlngth = x.length - 1
    for i in 0..xlngth
      xx[i] = x[i]
    end

    ylngth = y.length - 1
    for i in 0..ylngth
      yy[i] = y[i]
    end

    c = xx.zip(yy)
    if (x == y)
      hamming_distance = 0
    else  
      hamming_distance = 0
  
      c.each do |xx,yy|
        if (xx != yy )
          hamming_distance = hamming_distance + 1
        end 
      end
    end  
    hamming_distance
  end

  def self.greet(name)
  end

  def self.drink(beverage,size)
  end

end


