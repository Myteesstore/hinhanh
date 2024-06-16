import Replicate from 'replicate';
const replicate = new Replicate();

const input = {
    image: "https://replicate.delivery/pbxt/Ing7Fa4YMk6YtcoG1YZnaK3UwbgDB5guRc5M2dEjV6ODNLMl/cat.jpg",
    scale: 2,
    face_enhance: false
};

const output = await replicate.run("nightmareai/real-esrgan:350d32041630ffbe63c8352783a26d94126809164e54085352f8326e53999085", { input });
console.log(output)
//=> "https://replicate.delivery/pbxt/iVcx6825RF5EMppOandycFV8...# hinhanh
