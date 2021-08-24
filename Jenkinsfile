node {
  git branch: 'main', url: 'https://github.com/SiwatINC/multicraft-gui' // checks out Dockerfile and some project sources
  def image = docker.build "siwatinc/multicraft-gui:latest"
  image.push()
  docker.withRegistry("https://ghcr.io/v2") {
      image.push()
  }
  
}
